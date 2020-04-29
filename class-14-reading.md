[Home Page](https://sueduclos.github.io/reading-notes/)

## Class 14: Access Control (ACL)

### Links                                                       

- [RBAC Tutorial](https://www.youtube.com/watch?v=C4NP8Eon3cA)                                                           
- [5 Steps to RBAC](https://www.csoonline.com/article/3060780/security/5-steps-to-simple-role-based-access-control.html) 
- [Wiki - RBAC](https://en.wikipedia.org/wiki/Role-based_access_control)                                                 


### Vocabulary
- access control: In the fields of physical security and information security, this refers to the selective restriction of access to a place or other resource 
- role based access control: Role-based access control (RBAC) is a policy-neutral access-control mechanism defined around roles and privileges. The components of RBAC such as role-permissions, user-role and role-role relationships make it simple to perform user assignments.
- capabilities: A capability (known in some systems as a key) is a representation of some set of access rights. Typically, these access rights are CRUD operations on a certain model.

### Discussion Questions:

#### 1. Why is access control important? Describe an application that would need access control.
It restrict certain resources from being seen, changed or deleted by certain individuals. An app that retains any data. 

#### 2. What is a role used for?
To define what category the user falls into. Each user role (admin, editor, user, guest, etc) defines what CRUD operations (or capabilities) are accessible to that user. 

#### 3. Why is role based access control more scalable than discretionary or mandatory access control? 
It's more scable because you can add and delete roles based on need without largely affecting user data.
