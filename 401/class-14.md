# Read 14

## Review

When is Basic Authorization used vs. Bearer Authorization?
Bearer auth uses tokens, which is not only more secure, but should be used when user needs access to sensitive information/permissions.

- What does the JSON Web Token package do?
Transmit data as an object that can be signed, and then verified.

- What considerations should we make when creating and storing a SECRET?
Should not be guessable, and should not be available in the end release, meaning it should be saved in the .env


## Preview

### RBAC

RBAC is nothing more than the idea of assigning system access to users based on their role within an organization. The system needs of a given workforce are analyzed, with users grouped into roles based on common job responsibilities and system access needs. Access is then assigned to each person based strictly on their role assignment. With tight adherence to access requirements established for each role, access management becomes much easier.

### RBAC in 5 steps

1. Inventory your systems
2. Analyze your workforce and create roles
3. Assign people to roles
4. Never make one-off changes
5. Audit

