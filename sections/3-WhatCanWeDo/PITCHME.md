@snap[north-west]
#### What Can We Do?
#### **Mitigations**
@snapend

Show STRIDE table with new column, common mitigations

@ul
- S : Appropriate authentication. Don't store secrets.
- T : Appropriate authorization. HMACs. Digital signatures.
- R : Audit trails. Timestamps.
- I : Encryption. Privacy-enhanced protocols.
- D : Filtering. Throttling.
- E : Least privilege.
@ulend


Note:
- Don't have time to go into specifics, but here are some high-level common mitigations.
- Authentication is confirming someone is who they say they are.
- Authorization is controlling who can do what.
- Hash Message Authentication Code - a checksum

---

@snap[north-west]
#### What Can We Do?
#### *Digging Deeper*
@snapend

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
#### **Prioritising Threats**
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