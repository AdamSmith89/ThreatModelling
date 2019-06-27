---?image=assets/img/thinking2.jpg&size=150%
@snap[text-orange text-16]
3. What Can We Do?
<br><br><br>
@snapend

@snap[south-east text-02 text-orange]
Photo by [Ishan Gupta](https://unsplash.com/@ishang?utm_source=unsplash&utm_medium=referral&utm_content=creditCopyText) on [Unsplash](https://unsplash.com/search/photos/thought?utm_source=unsplash&utm_medium=referral&utm_content=creditCopyText)
@snapend

Note:
- Start thinking about anti-tamper
- Using privacy-enhanced protocols
- Adding extra authentication
- etc. etc. likely project specific

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
    <td><b>@color[#E58537](S)</b>poofing</td>
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
    <td><b>@color[#E58537](T)</b>ampering</td>
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
    <td><b>@color[#E58537](R)</b>epudiation</td>
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
    <td><b>@color[#E58537](I)</b>nformation Disclosure</td>
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
    <td><b>@color[#E58537](D)</b>enial of Service</td>
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
    <td><b>@color[#E58537](E)</b>levation of Privilege</td>
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

@snap[west fragment text-06 span-40]
@fa[windows fa-8x]
<br>Reinforce the window!
@snapend
@snap[midpoint fragment text-06 span-40]
@fa[bell fa-8x]
<br>Add an alarm system!
@snapend
@snap[east fragment text-06 span-40]
@fa[door-open fa-8x]
<br>Forgot about the key...
@snapend

Note:
Last thing to mention is 2nd/3rd order mitigations.
Attackers target the weakest link.
Cover all 1st order threats before moving on.

---
@snap[north-west]
#### What Can We Do?
@snapend

@snap[text-06]
<table>
  <col width="300">
  <col width="300">
  <col width="300">
  <tr>
    <th>Interaction</th>
    <th>Threat</th>
    <th>Mitigation</th>
  </tr>
  <tr>
    <td>Some interaction</td>
    <td>Threat posed</td>
    <td class="fragment">Mitigation</td>
  </tr>
  <tr>
    <td>Some interaction</td>
    <td>Threat posed</td>
    <td class="fragment">Mitigation</td>
  </tr>
  <tr>
    <td>Some interaction</td>
    <td>Threat posed</td>
    <td class="fragment">Mitigation</td>
  </tr>
  <tr>
    <td>Some interaction</td>
    <td>Threat posed</td>
    <td class="fragment">Mitigation</td>
  </tr>
  <tr>
    <td>Some interaction</td>
    <td>Threat posed</td>
    <td class="fragment">Mitigation</td>
  </tr>
  <tr>
    <td>Some interaction</td>
    <td>Threat posed</td>
    <td class="fragment">Mitigation</td>
  </tr>
</table>
@snapend

Note:
- So lets add our mitigations to our previous threat table.
- We do this so it's easy to keep track of and test later.
- Microsoft TM Tool

---
@snap[north-west]
#### What Can We Do?
@snapend

@img[shadow span-75](assets/img/tm_tool.png)

Note:
- Suggests threats based on components added to diagram
- Can generate reports

---
@snap[north-west]
#### What Can We Do?
@snapend

@ul
- Wait and See
- Easy fixes first
- Fix them all
- Bug bar
@ulend

Note:
- Got all your threat/mitigations. What do you do with them?!
- WaS : lightweight, can be catastrophic
- EFF : Fixes issues quickly, can be in a low priority area
- FTA : Time-consuimg. Should be the aim for new code, TM at design time so you mitigate before code writing
- BB : Choose a scoring mechanism (CVSS).
- Raise items for threats not mitigated. Tasks for design update, bugs for existing code, pbi's for new features.
- Might want to raise items/test cases for mitigated ones as well.