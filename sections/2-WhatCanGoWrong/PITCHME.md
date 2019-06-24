@snap[north-west]
#### What Can Go Wrong?
@snapend

<table>
  <col width="500">
  <col width="100">
  <tr class="fragment">
    <th><b>S</b>tride</th>
    <th>@fa[database]</th>
  </tr>
  <tr class="fragment">
    <th><b>T</b>ampering</th>
    <th>@fa[chalkboard]</th>
  </tr>
    <tr class="fragment">
    <th><b>R</b>epudiation</th>
    <th>@fa[arrow-up]</th>
  </tr>
    <tr class="fragment">
    <th><b>I</b>nformation Disclosure</th>
    <th>@fa[database]</th>
  </tr>
    <tr class="fragment">
    <th><b>D</b>enial of Service</th>
    <th>@fa[database]</th>
  </tr>
    <tr class="fragment">
    <th><b>E</b>levation of Privilege</th>
    <th>@fa[database]</th>
  </tr>
</table>

Note:
- Now the fun (scary) part!
- Could get everyone to think of threats.
- Going to suggest using STRIDE

---
@snap[north-west]
#### What Can Go Wrong?
#### *Spoofing*
@snapend

@snap[north-east span-50 fragment]
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
#### What Can Go Wrong? *Tampering*
@snapend

@snap[north-east span-100 fragment]
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
#### What Can Go Wrong? *Repudiation*
@snapend

@snap[north-east span-100 fragment]
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
#### What Can Go Wrong? *Information Disclosure*
@snapend

@snap[north-east span-100 fragment]
<br>
@quote[Exposing information to people who aren't supposed to see it](Adam Shostack)
@snapend

---
@snap[north-west]
#### What Can Go Wrong? *Denial of Service*
@snapend

@snap[north-east span-100 fragment]
<br>
@quote[Preventing a system from providing service](Adam Shostack)
@snapend

---
@snap[north-west]
#### What Can Go Wrong? *Elevation of Privilege*
@snapend

@snap[north-east span-100 fragment]
<br>
@quote[When a program of user is technically able to do things they are not supposed to](Adam Shostack)
@snapend