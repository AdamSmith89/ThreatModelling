## Threat Modelling
@snap[fragment]
### *Sooner The Better, But Better Late Than Never*
@snapend

Note:
- Great quote from OWASP

---

@snap[north span-100]
### Why Threat Model
@snapend

- Find security bugs early
- Helps drive-out Security Requirements
- Build better products
- Makes us think about Security!

Note:
- You may be thinking, why do I want to add more overhead to our process!
- SecREq: Is this necessary? Do we need to design for securing X?
- Driving out requirements and spotting bugs before we've written any code reduces re-work at later, more expensive, stages of dev.

---
@title[Agenda]

@snap[north span-100]
### 4 Key Questions
@snapend

@snap[west span-100]
@ol[spaced]
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
@fa[play]@note[Part of design for new code (features/bugs)]
@snapend

@snap[midpoint fragment]@note[It should be updated as design changes (we are bad at this)]
@fa[sync-alt]
@snapend

@snap[east fragment]
@fa[flag-checkered]
@ul
- @note[Review at the end to ensure it still matches (we are bad at this)]
@ulend
@snapend

@snap[south fragment]
@fa[cloud-meatball]
@note[Ideally legacy system should be TM'd (not sure on best approach here! per-team decision? Architect role, tech debt backlog, whole team smash it in a day or two?)]
@snapend

Note:
- Look at it like TDD, write test-cases first (find threats first to create tests)
- Said before, fail fast!

---

@snap[north span-100]
### Key Takeaways
@snapend

@snap[midpoint]
@ul
- 4 Key Questions
- STRIDE
- Threat Model should be a living diagram through feature development
@ulend
@snapend

Note:
- Remember at least this!
- Can anyone remember the questions?
- Can anyone remember STRIDE?

---

@snap[midpoint]
Any questions?
@snapend

---

@snap[north span-100]
### Useful Resources
@snapend

- CAPEC
- CVSS calculator
- Threat Modelling by Adam Shostack