### 3. What Can We Do?

---

@snap[north-west]
#### What Can We Do?
@snapend

@snap[text-06]
<table>
  <col width="250">
  <col width="500">
  <tr>
    <th/>
    <th>Typical Mitigations</th>
  </tr>
  <tr>
    <td><b>@color[#5289F7](S)</b>poofing</td>
    <td>
        @snap[fragment]
        @ul[](false)
        - Appropriate authentication
        - Don't store secrets
        @ulend
        @snapend
    </td>
  </tr>
  <tr>
    <td><b>@color[#5289F7](T)</b>ampering</td>
    <td>
        @snap[fragment]
        @ul[](false)
        - Appropriate authorization
        - HMACs
        - Digital signatures
        @ulend
        @snapend
    </td>
  </tr>
    <tr>
    <td><b>@color[#5289F7](R)</b>epudiation</td>
    <td>
        @snap[fragment]
        @ul[](false)
        - Audit trails
        - Timestamps
        @ulend
        @snapend
    </td>
  </tr>
  <tr>
    <td><b>@color[#5289F7](I)</b>nformation Disclosure</td>
    <td>
        @snap[fragment]
        @ul[](false)
        - Encryption
        - Privacy-enhanced protocols
        @ulend
        @snapend
    </td>
  </tr>
    <tr>
    <td><b>@color[#5289F7](D)</b>enial of Service</td>
    <td>
        @snap[fragment]
        @ul[](false)
        - Filtering
        - Throttling
        @ulend
        @snapend
    </td>
  </tr>
    <tr>
    <td><b>@color[#5289F7](E)</b>levation of Privilege</td>
    <td>
        @snap[fragment]
        @ul[](false)
        - Least privilege
        @ulend
        @snapend
    </td>
  </tr>
</table>
@snapend

Note:
- Don't have time to go into specifics, but here are some high-level common mitigations.
- Authentication is confirming someone is who they say they are.
- Authorization is controlling who can do what.
- Hash Message Authentication Code - a checksum

---

@snap[north-west]
#### What Can We Do?
@snapend

@snap[north]
@fa[sort-numeric-down]
@snapend

@snap[west span-200 fragment]
@fa[windows]
@snapend
@snap[midpoint span-200 fragment]
@fa[bell]
@snapend
@snap[east span-200 fragment]
@fa[door-open]
@snapend

Note:
Should I discuss 1st/2nd/3rd order mitigations?
Window smashing, don't forget about the key under the mat!
Cover all 1st order threats before moving on.
Attackers target the weakest link.

---

@snap[north-west]
#### What Can We Do?
@snapend

Organise threats so it's easy to track mitigations - threat modelling tool!
Now add mitigations for the threats you have found.

Note:
- Need to organise threats you've found, assumptions made and mitigations proposed
- I'd suggest the TM tool for that

---

@snap[north-west]   
#### What Can We Do?
#### *Prioritising Threats*
@snapend

@ul
- Wait and See
- Easy fixes first
- Fix them all
- Bug bar
@ulend

Note:
- WaS : lightweight, can be catastrophic
- EFF : Fixes issues quickly, can be in a low priority area
- FTA : Time-consuimg. Should be the aim for new code, TM at design time so you mitigate before code writing
- BB : Choose a scoring mechanism (CVSS).
- Raise items for threats not mitigated. Tasks for design update, bugs for existing code, pbi's for new features.
- Might want to raise items/test cases for mitigated ones as well.