[Live URL](https://mujahedyousef.github.io/advanced-js-reading-notes.-/day_7/class_7.html)

# Reading: Access Control (ACL)

--------
|  Term  |   Meaning |
|--- |--- |
|encryption| Is a means of securing digital data using one or more mathematical techniques, along with a password or "key" used to decrypt the information.  |
|token|   Is a software device required for a user to access an application or a network system in a more secure way.      |
|bearer|  (also called token authentication) is an HTTP authentication scheme that involves security tokens called bearer tokens.    |
|secret|    Programmably private tokens with encrypted data.      |
|JSON Web Token|   is a means of representing claims to be transferred between two parties. The claims in a JWT are encoded as a JSON object that is digitally signed using JSON Web Signature (JWS) and/or encrypted using JSON Web Encryption.      |
|||
-------

## Role-Based Access Control (RBAC)

> Is the modern role-based permissions management model that helps in managing access at both the broad as well as the granular level by aligning the assigned permissions role with the organizational role of the user. It helps in avoiding access leaks and, thereby, reducing the risk of data and information security breaches.

* ## Benefits of RBAC

1. create systematic, repeatable assignment of permissions.

1. easily audit user privileges and correct identified issues.

1. quickly add and change roles, as well as implement them across APIs.

1. cut down on the potential for error when assigning user permissions.

1. integrate third-party users by giving them pre-defined roles.

1. more effectively comply with regulatory and statutory requirements for confidentiality and privacy.

* ## primary rules are defined for RBAC
>
>* Role assignment.
>* Role authorization.
>* Permission authorization.

* ## RBAC implementation

1. Inventory your systems.
2. Analyze your workforce and create roles.
3. Assign people to roles.
4. Never make one-off changes.
5. Audit.

----
![AuthRBAC](/day_7/Authorization_RBAC.png)
