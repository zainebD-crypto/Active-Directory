# Active Directory (AD)

From one beginner to another: curiosity is your biggest weapon in cybersecurity.

These documents reflect what I learned while trying to understand concepts like Active Directory and beyond. They’re not authoritative, just a snapshot of my learning journey.

If this helps you take your first steps, mission accomplished.
**Good luck — thank me later!**


#### Active directory is the backbone of the corporate world. 
#### Microsoft Active Directory serves as the core infrastructure of corporate networks, enabling centralized control over users and devices.


***Windows Domain:*** Windows Domain is a group of users and computers under the adminsitrations of a given business.

**The server that runs the Active Directory services is known as a Domain Controller (DC).**
- *Advantages of having a configured windows domain:*
    1. **Centralised identity management:** All users across the network can be configured     from Active Directory with minimum effort.
    2. **Managing security policies:** You can configure security policies directly from Active Directory and apply them to users and computers across the network as needed.
       
       ![image alt](https://github.com/zainebD-crypto/Active-Directory/blob/main/img_1769199579688_7e7b8d5c088af.png?raw=true)
       

Active Directory stores information about objects on the network such as users,computers, printers, groups and applications. It provides a centrilized database for authentication and authorization, enabling adminstrators to manage acces to network ressources and enforces security policies.

![image alt](https://github.com/zainebD-crypto/Active-Directory/blob/main/img_1769200174303_4e85e2f94129e.png?raw=true)

### Active Directory Domain Service (AD DS)
the AD DS hols the information of all the objects on your network.

Active Directory has two types of groups:
- **Security groups:** Used to assign permissions to shared resources.
- **Distribution groups:** Used to create email distribution lists.

***Security groups:***
==>Security groups are a way to collect user accounts, computer accounts, and other groups into manageable units.

- Domain admins: users of this group have administrative privileges over the entire domain. By default, they can administer any computer on the domain, including the DCs.
- Server Operators: Users in this group can administer Domain Controllers.
- Backup operators: Users in this groupe are allowed to access any file, ignoring their permissions. They are used to perform backups data of computers.
- Account Operators: Users in this group can create or modify other accounts in the domain.
- Domain Users: All ecisting user accounts in the domain.
- Domain Computers: All existing computers in the domain.
- Domain Controller:Domain Controllers allow you to manage the Active Directory Domain 

**Organizational Units(OUs):** container objects that allow you to classify users and machines.

Security Groups vs OUs:
**OUs:** applying policies to users and computers 
**Security groups:** grant permissions over resources.
### Key components and Concepts:
Understanding the key components of *Active Directory is crucial. 
- A **Domain** fundamental unit of organisation in Active Directory. It represents a logical grouping of users, computers and other resoureces that shares a common directoy database and security policies. A domain has a unique name and is managed by one or more domain controllers.
![image alt](https://github.com/zainebD-crypto/Active-Directory/blob/main/img_1769259759296_04122869d8bf4.png?raw=true)


- A **domain controller** is a server that manages security authentication requests in a Windows Server network. It stores user account information and controls access to resources on the network. It is a critical component for managing and securing a network infrastructure.
![image alt](https://github.com/zainebD-crypto/Active-Directory/blob/main/img_1769259809987_c453d71d887188.png?raw=true)

- An **Organisational Unit (OU)**: is a container within a domain that allows administrators to organize and manage users, computers and other objects in a hierarchical structure. OUs can be used to delegate administrative control, apply group policies and simplify managment tasks.
![image alt](https://github.com/zainebD-crypto/Active-Directory/blob/main/img_1769260017666_01d95b833189c8.png?raw=true)

A **Group Policy**: a powerful feature of active directory that allows administrators to centrally manage user and computer settings. Group policies can be applied to domains, OUs or individual users and computers. They can be used to configure a wide range of settings:
    1.Password policies
    2.software installation
    3. security settings 
    4.desktop customization

![image alt](https://github.com/zainebD-crypto/Active-Directory/blob/main/img_1769260809686_37d9afe4a68378.png?raw=true)
    

- An **Active Directory Schema**: The active directory defines the structure and attributes of objects that can be stored in the directory. It specifies the classes of objects and the propreties that can be associated with each object.
![image alt](https://github.com/zainebD-crypto/Active-Directory/blob/main/img_1769261044792_9349454a93544.png?raw=true)

- **Trust Relationships** allows users in one domain to access resources in another domain. They are essential for enabling collaborration and resource sharing between different domains. Trusts can be one-way or two-way.
![image alt](https://github.com/zainebD-crypto/Active-Directory/blob/main/img_1769261313961_d4c1e49cbb4f8.png?raw=true)

- **Azure Active Directory (Azure AD)** is microsoft's cloud-based identity and access management service. While it shares the Active Directory name, it is a distinct service from on-premises Avtive Directory Domain Services( AD DS). Azure AD os designed for managing identities and access to cloud applications and services. It can be integrated with on-premises AD DS to provide a hybrid identity solution.
![image alt](https://github.com/zainebD-crypto/Active-Directory/blob/main/img_1769261904097_280177ea2b6d2.png?raw=true)


Enumerating the benefits of unsing AD : 

1. Centralized Maagment: provides a central point of control for managing objects and other resources on the network. This simplifies adminitration and reduces the risque of inconsistencies and errors.

2. Enhanced Security: AD enables administrators to enforce security policies consistently across the organisaion. This helps to protect sensitve data and prevent unauthorized access.

3. Simplified USer Managment: AD simplifies user maangment tasks such as creating new user accounts, resetting passwords and managing user permissions.

4. Improved compliance: AD helps organizations to meet regularity compliance requirements by providing a centralized audit trail of user activity and access to resources.

5. Single Sign-On (SSO): AD enables users to access mutiple applications and services with a signle set of credentials. This reduces the rish of password fatigue.

6. Scalability and Reliability: AD is designed to be reliable. IT can support large numbers of users and computers.

### Common Use Cases:

Active Directory is used in a wide range of scenarios:

- **User Authentication and Authorization:** AD is used to authenticate users and authorize access to network resources.

- **Computer Management:** AD is used to manage computer settings and configurations.

- **Software Deployment:** AD is used to deploy software applications to users and computers.

- **Group Policy Management:** AD is used to manage group policies and enforce security settings.

- **Remote Access:** AD is used to provide secure remote access to network resources.

- **Identity and Access Management (IAM):** AD is used as a core component of an organization's IAM strategy.


## Conclusion
Active Directory is a powerful and versatile directory service that provides a foundation for managing users, computers and resources in a Windows domain environment. Its centralized management capabilities, enhanced security features, and simplified user management capabilities, enhanced security features, and simplified user management tools make it an essential component of modern It infrasturcture. While Azure AD is increasingly important for cloud-based identity management on-premises Active Directory remains a critical component for many organizations, especially those with hybrid environments. Understanding the core concepts and benefits of Active Directory is crucail for IT professionals who are responsible for managing and securing their organization's network.

![image alt](https://github.com/zainebD-crypto/Active-Directory/blob/main/img_1769263853467_3911158ba3f128.png?raw=true)
