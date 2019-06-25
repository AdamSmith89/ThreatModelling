### 2. What Can Go Wrong?

Note:
- Framework to help you focus on the type of threats you might face
- STRIDE threats are purposefully the opposite of properties we would like in our system
- Easy to remember and apply for good results
- there are other ways
  - Attack Trees (show example?)
  - Attack Libraries (show example?)

  - Trees : Start with goal (repudiate data etc.) and then leaf nodes are how that is achieved
    - Can be harder to get started.
    - Doesn't lend itself well to our process.
    
- Libraries : A collection of commo attacks against a system.
    - High-level can be too abstract
    - Low-level can be too specific (or need to create your own)

---
@snap[north-west]
#### What Can Go Wrong?
@snapend

@snap[text-06]
<table>
  <col width="250">
  <col width="500">
  <col width="150">
  <tr>
    <th/>
    <th>Definition</th>
    <th>Principle Violated</th>
  </tr>
  <tr>
    <td class="fragment"><b>S</b>poofing</td>
    <td class="fragment">Pretending to be something or someone you are not</td>
    <td class="fragment">Authenticity</td>
  </tr>
  <tr>
    <td class="fragment"><b>T</b>ampering</td>
    <td class="fragment">Modifying something you aren't supposed to modify</td>
    <td class="fragment">Integrity</td>
  </tr>
    <tr>
    <td class="fragment"><b>R</b>epudiation</td>
    <td class="fragment">Claiming you didn't do something</td>
    <td class="fragment">Non-Repudiation</td>
  </tr>
    <tr>
    <td class="fragment"><b>I</b>nformation Disclosure</td>
    <td class="fragment">Exposing information to people who aren't supposed to see it</td>
    <td class="fragment">Confidentiality</td>
  </tr>
    <tr>
    <td class="fragment"><b>D</b>enial of Service</td>
    <td class="fragment">Preventing a system from providing service</td>
    <td class="fragment">Availability</td>
  </tr>
    <tr>
    <td class="fragment"><b>E</b>levation of Privilege</td>
    <td class="fragment">When a program or user is technically able to do things they are not supposed to</td>
    <td class="fragment">Authorization</td>
  </tr>
</table>
@snapend

Note:
- STRIDE is the opposite of desirable properties of your system
- there are typical victims of each threat
- Ask for examples before showing.
- Spoofing
  - Processes, people
  - Creating a file before the real process
  - Naming malicious process same as real process
- Tampering
  - Data stores, data flows
  - Modifying files a process relies on
  - Modifying process memory
- Repudiation
  - Process
  - Use someone else's account
  - Attack logs
- Information Disclosure
  - Processes, data stores, data flows
  - Usually the target of another attack
  - (Obvious) Allowing access to files
  - (Other) File names (People To Fire.doc)
- Denial of Service
  - Processes, data stores, data flows
  - Creating many network connections/requests
  - Tricking a process to consume a resource
- Elevation of Privilege
  - Process
  - Allowing a standard user to run code as admin.

---
@snap[north-west span-100]
#### What Can Go Wrong?
@snapend

@snap[midpoint span-200]
@img[shadow](assets/img/acme-dfd-trust.PNG)
@snapend

Note:
- Can we think of any more threat?

---
@snap[north-west]
#### What Can Go Wrong?
@snapend

@ul
- List a few of the other threats.
@ulend