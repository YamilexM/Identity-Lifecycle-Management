# Microsoft Entra ID Identity Lifecycle Management

## Project Overview

In this lab, I practiced a basic user offboarding workflow in Microsoft Entra ID.

Building on my previous labs, Taylor Morgan had already been created, licensed, assigned a directory role, and added to a security group. In this project, I worked through the process of removing that access and transitioning the account into an inactive state.

The goal was to better understand the "leaver" stage of the identity lifecycle and how access can be removed when a user no longer needs access to an environment.

## Technologies Used

- Microsoft Entra ID
- Microsoft Azure
- Identity and Access Management (IAM)
- User Lifecycle Management

## What I Practiced

- Reviewing a user's current access before offboarding
- Removing group membership
- Removing assigned directory roles
- Removing a Microsoft Entra ID P2 license
- Disabling a user account
- Revoking user sessions
- Verifying the user's final access state
- Documenting an offboarding workflow

## Step 1: Review the User Before Offboarding

Before making any changes, I reviewed **Taylor Morgan's** account in Microsoft Entra ID.

At the beginning of the offboarding process, the account showed:

- **Account Status:** Enabled
- **Group Memberships:** 1
- **Assigned Roles:** 1
- **Assigned Licenses:** 1

This gave me a clear view of the access that needed to be removed during the offboarding process.

![User Before Offboarding](images/01-user-before-offboarding.png)

## Step 2: Remove User Access

As part of the offboarding workflow, I removed the access that had previously been assigned to the user.

This included:

- Removing the user's security group membership
- Removing the assigned directory role
- Removing the Microsoft Entra ID P2 license
- Disabling the user account

These steps helped me practice reducing access as part of the user lifecycle process.

## Step 3: Revoke User Sessions

After the account was disabled and access was removed, I used the **Revoke sessions** option in Microsoft Entra ID.

This action was used to revoke the user's existing sessions and require the account to authenticate again before accessing Microsoft services.

![Revoke User Sessions](images/04-revoke-user-sessions.png)

## Step 4: Verify the Offboarded Account

After completing the offboarding steps, I returned to Taylor Morgan's account overview to verify the final state.

The account showed:

- **Account Status:** Disabled
- **Group Memberships:** 0
- **Assigned Roles:** 0
- **Assigned Licenses:** 0

This confirmed that the user's previously assigned access had been removed and the account was left in a disabled state.

![User Offboarding Complete](images/05-user-offboarding-complete.png)

## Skills Practiced

- Microsoft Entra ID
- Identity and Access Management
- Identity Lifecycle Management
- User Offboarding
- Access Removal
- License Management
- Security Group Management
- Directory Role Management
- Session Revocation
- Account Verification
- Technical Documentation

## What I Learned

This lab helped me understand that identity management does not stop after a user is created.

I practiced the offboarding side of the identity lifecycle by reviewing an existing user's access, removing previously assigned permissions and memberships, disabling the account, and revoking user sessions.

This helped me better understand how user provisioning and deprovisioning work together as part of Identity and Access Management.
