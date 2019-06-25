@snap[north-west]
#### What Can Go Wrong?
@snapend

@snap[midpoint]
Show diagram we just finished
@snapend

Note:
- What threats can you think of?
- Write them on a board!

---
@snap[north-west]
#### What Can Go Wrong?
#### *Spoofing*
@snapend

@snap[north-east span-60 fragment]
<br>
@quote[Pretending to be something or someone you are not](Adam Shostack)
@snapend

@snap[west]
@ul
- Violates authentication
- Processes, people
- Creating a file before the real process
- Naming malicious process same as real process
@ulend
@snapend

Note:
- STRIDE is the opposite of desirable properties of your system
- There are typical victims of each threat
- Ask for examples before showing.

---
@snap[north-west]
#### What Can Go Wrong?
####*Tampering*
@snapend

@snap[north-east span-60 fragment]
<br>
@quote[Modifying something you aren't supposed to modify](Adam Shostack)
@snapend

@snap[west]
@ul
- Violates integrity
- Data stores, data flows
- Modifying files a process relies on
- Modifying process memory
@ulend
@snapend

Note:
- 

---
@snap[north-west]
#### What Can Go Wrong?
#### *Repudiation*
@snapend

@snap[north-east span-60 fragment]
<br>
@quote[Claiming you didn't do something](Adam Shostack)
@snapend

@snap[west]
@ul
- Violates non-repudiation
- Process
- Use someone else's account
- Attack logs
@ulend
@snapend

Note:
- 

---
@snap[north-west]
#### What Can Go Wrong?
#### *Information Disclosure*
@snapend

@snap[north-east span-60 fragment]
<br>
@quote[Exposing information to people who aren't supposed to see it](Adam Shostack)
@snapend

---
@snap[north-west]
#### What Can Go Wrong?
#### *Denial of Service*
@snapend

@snap[north-east span-60 fragment]
<br>
@quote[Preventing a system from providing service](Adam Shostack)
@snapend

---
@snap[north-west]
#### What Can Go Wrong?
#### *Elevation of Privilege*
@snapend

@snap[north-east span-60 fragment]
<br>
@quote[When a program of user is technically able to do things they are not supposed to](Adam Shostack)
@snapend

---

@snap[north-west]
#### What Can Go Wrong?
#### *Why STRIDE?*
@snapend

@snap[midpoint]
@ul
- Framework to help you focus on the type of threats you might face
- STRIDE threats are purposefully the opposite of properties we would like in our system
- Easy to remember and apply for good results
- There are other ways
  - Attack Trees (show example?)
  - Attack Libraries (show example?)
@ulend
@snapend

Note:
- Trees : Start with goal (repudiate data etc.) and then leaf nodes are how that is achieved
    
- Libraries : A collection of commo attacks against a system.
    - High-level can be too abstract
    - Low-level can be too specific (or need to create your own)