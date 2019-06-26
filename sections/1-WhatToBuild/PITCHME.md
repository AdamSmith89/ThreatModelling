---?image=assets/img/architect.jpg&size=cover
@css[text-white](### 1. What Are We Building?)

@snap[south-east text-02]
Photo by [Daniel McCullough](https://unsplash.com/@d_mccullough?utm_source=unsplash&utm_medium=referral&utm_content=creditCopyText) on [Unsplash](https://unsplash.com/search/photos/architect?utm_source=unsplash&utm_medium=referral&utm_content=creditCopyText)
@snapend

Note:
- Suggest using a DFD. Familiar to most people. Problems/threats tend to follow the data flow. Allows you to focus attention on the important parts of the system.
- If data can go either one place or another, add both!
- Can split into multiple diagrams

---
@snap[north-west span-100]
#### What Are We Building?
@snapend

@snap[midpoint span-200]
@img[shadow](assets/img/acme-dfd-no-trust.PNG)
@snapend

Note:
- Not much different from a normal DFD
- Difficult to find all the threats
- Can we find any? Write them on a board!
- Next we are going to add trust boundaries

---
@snap[north-west span-100]
#### What Are We Building?
@snapend

@snap[midpoint span-200]
@img[shadow](assets/img/acme-dfd-trust.PNG)
@snapend

Note:
- Show who controls what. Can be anything from physical locations to privilege levels on a single machine
- Trust Boundaries Helps you focus on where threats are likely to be found
- Sometimes known as Attack Surfaces
- This is the key difference between standard diagrams
- Any more threats that can be found?