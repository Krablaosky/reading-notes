# Access Control(ALC)

## [5 steps to RBAC](https://www.csoonline.com/article/3060780/5-steps-to-simple-role-based-access-control.html)

1. What is Role Based Access Control (RBAC) and why do we care?

  Role-Based Access Control (RBAC) is a method of access control that defines permissions and access rights based on roles assigned to users. We care about RBAC because it provides a systematic and scalable approach to managing access to resources within an organization. It simplifies administration, improves security, and reduces the risk of unauthorized access.

2. Describe a Role/Permission heirarchy that you might implement using RBAC.

  In an RBAC implementation, a role/permission hierarchy can be structured based on the organization's needs. For example:

     * Basic User: Has read-only access to certain resources.
     * Power User: Has read and write access to specific resources.
     * Manager: Has access to view, edit, and delete resources across multiple departments.
     * Administrator: Has full control and unrestricted access to all resources and permissions.

3. What approach might you take to implement RBAC?
  
  To implement RBAC, you can follow these steps:

    * Identify Roles: Determine the roles within the organization and the access permissions associated with each role.
    
    * Assign Roles: Assign appropriate roles to individual users based on their job responsibilities and access requirements.
    
    * Define Permissions: Define the permissions and access rights associated with each role.
    
    * Implement Role Mapping: Establish a mechanism to map roles to users and their corresponding permissions.
    
    * Regularly Review and Update: Continuously review and update role assignments and permissions as job roles change or when new resources are added.

## [wiki - RBAC](https://en.wikipedia.org/wiki/Role-based_access_control)

1. If Authentication is “you are who you say you are,” what is Authorization?

  Authentication refers to the process of verifying the identity of a user, confirming that they are who they claim to be. Authorization, on the other hand, is the process of granting or denying access rights and permissions to authenticated users based on their roles, responsibilities, and other relevant factors.

2. Name three primary rules defined for RBAC.

  Three primary rules defined for RBAC are:

    * Role-Based: Access control decisions are based on the roles assigned to users.
    
    * Permission-Based: Access control is defined by the permissions associated with each role.
    
    * Least Privilege: Users are granted the minimum privileges necessary to perform their tasks, reducing the risk of unauthorized access.

3. Describe RBAC to a non-technical friend.

  RBAC can be explained to a non-technical friend as a system that controls who can access what within an organization. It uses roles to define what different users can do and what resources they can access. RBAC ensures that each user has the right level of access and permissions to perform their job while maintaining security by restricting unauthorized access.

## [RBAC tutorial](https://www.youtube.com/watch?v=C4NP8Eon3cA)

1. What Are access rights Associated with? The User? or The Role? Explain.

  Access rights are associated with the Role in RBAC. Users are assigned roles, and these roles determine the access rights and permissions granted to the users. Instead of assigning access rights directly to individual users, RBAC simplifies management by associating them with roles.
  
2. Access Rights, or Authorization, is activated after a user successfully does what?

  Access rights, or authorization, are activated after a user successfully authenticates (proving their identity) and is assigned a specific role. Once authenticated and assigned a role, the user's access rights are determined by the permissions associated with that role.

3. Explain how RBAC might benefit a business.

  RBAC can benefit a business in several ways:

    * Improved Security: RBAC ensures that users only have access to the resources they need to perform their job, reducing the risk of unauthorized access and data breaches.

    * Simplified Administration: RBAC simplifies the process of managing user access by grouping permissions into roles. This makes it easier to assign and modify access rights as users change roles or responsibilities.

    * Compliance and Auditing: RBAC provides a structured approach to access control, which helps businesses demonstrate compliance with regulatory requirements. It also enables easier auditing and tracking of access rights and permissions.
    
    * Increased Efficiency: RBAC streamlines access management, reducing administrative overhead and allowing employees to focus on their core tasks rather than dealing with access-related issues.