@snap[text-gold text-20]
Threat Modelling
@snapend
@snap[fragment]
### *Sooner The Better, But Better Late Than Never*
@snapend

Note:
- Great quote from OWASP

---
@snap[north span-100]
### Why Threat Model
@snapend

@snap[north-west fragment]
<br>
Fail Fast
@snapend

@snap[north-east fragment]
<br><br>
Define security requirements
@snapend

@snap[west fragment]
<br>
Build better products
@snapend

@snap[south-east fragment]
Makes us think Security!
@snapend

Note:
- Any suggestions?
- SecREq: Is this necessary? Do we need to design for securing X?

---
@title[Agenda]

@snap[north span-100]
### 4 Key Questions
@snapend

@snap[west]
@ol
- What are we building?
- What can go wrong?
- What can we do about it?
- Did we do a good job?
@olend
@snapend

---?include=sections/1-WhatToBuild/PITCHME.md
---?include=sections/2-WhatCanGoWrong/PITCHME.md
---?include=sections/3-WhatCanWeDo/PITCHME.md
---?include=sections/4-HowDidWeDo/PITCHME.md

---
@snap[north span-100]
### When To Threat Model
@snapend

@snap[west fragment]
@fa[play fa-4x]
@snapend

@snap[midpoint fragment]
@fa[sync-alt fa-4x]
@snapend

@snap[east fragment]
@fa[flag-checkered fa-4x]
@snapend

@snap[north fragment]
@fa[cloud-meatball fa-4x]
@snapend

@snap[south text-08 span-120 fragment]
@quote[Threat Modelling empowers Testing;<br>Testing empowers Threat Modelling](Adam Shostack)
@snapend

Note:
- Part of design for new code (features/bugs)
- It should be updated as design changes (we are bad at this)
- Review at the end to ensure it still matches (we are bad at this)
- Ideally legacy system should be TM'd
  - Don't do it? Per-team decision? Architect role? TD backlog? Team smash it in a day or two?
- Look at it like TDD, write test-cases first (find threats first to create tests)
- Said before, fail fast!

---

@snap[north span-100]
### Key Takeaways
@snapend

@ul
- 4 Key Questions
- STRIDE
- Threat Model should be a living diagram through feature development
@ulend

Note:
- Remember at least this!
- Can anyone remember the questions?
- Can anyone remember STRIDE?

---
@snap[midpoint]
@fa[question fa-8x]
@snapend

---

@snap[north span-100]
### Useful Resources
@snapend

- CAPEC
- CVSS calculator
- Threat Modelling by Adam Shostack