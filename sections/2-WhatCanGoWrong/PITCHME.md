---?image=assets/img/iceberg3.jpg&size=cover
@snap[east text-orange text-16 move-right-50]
2. What Can Go Wrong?
@snapend

@snap[south-east text-02 text-orange]
Photo by [Viktor Jakovlev](https://unsplash.com/@apviktor?utm_source=unsplash&utm_medium=referral&utm_content=creditCopyText) on [Unsplash](https://unsplash.com/search/photos/risk?utm_source=unsplash&utm_medium=referral&utm_content=creditCopyText)
@snapend

Note:
- Introduce STRIDE
- Framework to help you focus on the type of threats you might face
- STRIDE threats are purposefully the opposite of properties we would like in our system
- Easy to remember and apply for good results
- there are other ways; focus on STRIDE today

---
@snap[north-west]
#### What Can Go Wrong?
@snapend

@snap[text-06]
<table>
  <col width="300">
  <col width="500">
  <col width="150">
  <tr>
    <th/>
    <th>Definition</th>
    <th>Principle Violated</th>
  </tr>
  <tr class="fragment">
    <td><b>@color[#E58537](S)</b>poofing</td>
    <td>Pretending to be something or someone you are not</td>
    <td>Authenticity</td>
  </tr>
  <tr class="fragment">
    <td><b>@color[#E58537](T)</b>ampering</td>
    <td>Modifying something you aren't supposed to modify</td>
    <td>Integrity</td>
  </tr>
    <tr class="fragment">
    <td><b>@color[#E58537](R)</b>epudiation</td>
    <td>Claiming you didn't do something</td>
    <td>Non-Repudiation</td>
  </tr>
    <tr class="fragment">
    <td><b>@color[#E58537](I)</b>nformation Disclosure</td>
    <td>Exposing information to people who aren't supposed to see it</td>
    <td>Confidentiality</td>
  </tr>
    <tr class="fragment">
    <td><b>@color[#E58537](D)</b>enial of Service</td>
    <td>Preventing a system from providing service</td>
    <td>Availability</td>
  </tr>
    <tr class="fragment">
    <td><b>@color[#E58537](E)</b>levation of Privilege</td>
    <td>When a program or user is technically able to do things they are not supposed to</td>
    <td>Authorization</td>
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
  - Assurance that someone cannot deny something
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
- STRIDE per interaction
- STRIDE per threat
- Don't worry about exactly which category a threat should be in.
  - Just a tool to help think of threats!
- Threats should be 5 * number of components in the system
- Don't think about mitigations

---
@snap[north-west]
#### What Can Go Wrong?
@snapend

@snap[text-06]
<table>
  <col width="350">
  <col width="450">
  <tr>
    <th>Interaction</th>
    <th>Threat</th>
  </tr>
  <tr class="fragment">
    <td>Database to Logs</td>
    <td>Users aren't tracked as database doesn't log session information</td>
  </tr>
  <tr class="fragment">
    <td>Front End(s) to Database</td>
    <td>SQL injection may cause a data leak</td>
  </tr>
  <tr class="fragment">
    <td>DB Admin to Database</td>
    <td>Many complex requests may impact performance</td>
  </tr>
  <tr class="fragment">
    <td>DB Users to Log Analysis</td>
    <td>Non-admin users can access logs</td>
  </tr>
  <tr class="fragment">
    <td>Web Clients to Front End(s)</td>
    <td>Existing authentication is weak</td>
  </tr>
  <tr class="fragment">
    <td>Front End(s) to Database</td>
    <td>Two routines allow any caller to run arbitrary code by design</td>
  </tr>
</table>
@snapend

Note:
Guess the STRIDE category
1. Repudiation: Don't know who was logged in!
2. Information disclosure
3. Denial of Service
4. Information disclosure / tampering
5. Spoofing
6. Elevation of Privilege