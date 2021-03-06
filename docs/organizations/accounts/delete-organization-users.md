---
title: Delete users from Visual Studio Team Services
description: Steps for how to delete or remove organization users from Visual Studio Team Services (VSTS) and removing users from a team or team project
ms.prod: devops
ms.technology: devops-accounts
ms.topic: conceptual
ms.assetid: d3a31878-a869-45a9-9bca-f46cc2682596
ms.manager: douge
ms.author: chcomley
author: chcomley
ms.date: 07/31/2018
monikerRange: 'vsts'
---


# Delete users from Visual Studio Team Services (VSTS)

**VSTS**

If a user no longer requires access to a team project or your VSTS organization, you can remove their access to a team project or your organization.

## Prerequisites

- You'll need [VSTS project collection administrator or organization owner permissions](../../organizations/security/set-project-collection-level-permissions.md?toc=/vsts/organizations/accounts/toc.json&bc=/vsts/organizations/accounts/breadcrumb/toc.json).

## Remove users from your VSTS organization

[!INCLUDE [temp](../../boards/_shared/new-agile-hubs-feature.md)]

# [New navigation](#tab/new-nav)

1. Sign in to your VSTS organization (```https://{yourorganization}.visualstudio.com```).

   [Why am I asked to choose between my work or school account and my personal account?](faq-create-organization.md#ChooseOrgAcctMSAcct)

2. Go to your VSTS admin settings.

    ![Open VSTS admin settings](../../_shared/_img/settings/open-admin-settings-vert.png)

3. Open the context menu **...** ,for the user to be removed, and select **Remove from organization**.

   ![Remove user from organization](_img/delete-user/remove-user-from-organization.png)

4. Choose **Remove** in the confirmation dialog.

   ![Confirm to remove existing user](_img/delete-user/confirm-remove-existing-user.png)

5. To make sure that you've removed the user completely, make sure they are not in any of your [security groups](../../organizations/security/add-users-team-project.md). 

   [Why don't users appear or disappear promptly in VSTS after I add or delete them in the Users hub?](faq-add-delete-users.md#users-delay)

6. If you deleted paid users who had Basic features, and you don't want to pay for these users, you must also [reduce these users in the Visual Studio Marketplace](../billing/buy-basic-access-add-users.md),so you're not charged in your next Azure billing cycle.

   > To reduce or cancel these users for the next month, you must make updates before the last day of the current month.
   > Your bill won't show these changes until the next month because paid users are monthly purchases.

# [Previous navigation](#tab/prev-nav)

1. Sign in to your VSTS organization (```https://{yourorganization}.visualstudio.com```).

   [Why am I asked to choose between my "work or school account" and my "personal account"?](faq-add-delete-users.md#ChooseOrgAcctMSAcct)

2. Go to the **Users** page.

3. Open the context menu **...** for the user to remove and select **Remove from organization**.

   ![![Remove user from organization](_img/delete-user/remove-user.png)
](_img/_shared/remove-from-organization-menu-selection.png)

4. Choose **Remove** in the confirmation dialog.

5. To make sure that you've removed the user completely, make sure they are not in any of your [security groups](../../organizations/security/add-users-team-project.md). 

   [Why don't users appear or disappear promptly in VSTS after I add or delete them in the Users hub?](faq-add-delete-users.md#users-delay)

6. If you deleted paid users who had Basic features, and you don't want to pay for these users, you must also [reduce these users in the Visual Studio Marketplace](../billing/buy-basic-access-add-users.md),so you're not charged in your next Azure billing cycle.

   > To reduce or cancel these users for the next month, you must make updates before the last day of the current month.
   > Your bill won't show these changes until the next month because paid users are monthly purchases.

---

>[!Note]
>Azure AD-backed organizations: Once you remove a user from Azure AD, you will not be able to assign artifacts (work items, pull requests, etc.) to this user anymore. However, we will preserve the history of artifacts that has already been assigned to this user.
>MSA-backed organizations: Once you remove a user from your MSA-backed VSTS organization, the user will remain within the tenant and can therefore be re-added at any time.

## Remove users from a team or team project

To remove users from a team project, remove them from the Teams groups they belong to or the Contributors group for the team project. See [Add users to a team project or specific team](../../organizations/security/add-users-team-project.md). From the Members page of a team group or security group, you can Remove a user.

# [New navigation](#tab/new-nav)

![Remove user from a security group](_img/delete-user/remove-user-from-project.png)

# [Previous navigation](#tab/prev-nav)

![Remove user from a security group](_img/delete-user/remove-user.png)

---

## Related articles

- [Add administrators, set permissions at the project-level or project collection-level](../../organizations/security/set-project-collection-level-permissions.md). 
- [Change individual permissions, grant select access to specific functions](../../organizations/security/change-individual-permissions.md)
- [Grant or restrict access to select features and functions](../../organizations/security/restrict-access.md)
- [Troubleshoot adding and deleting organization users in the VSTS user hub](faq-add-delete-users.md)
- [Troubleshoot adding members to team projects in Visual Studio Team Services (VSTS)](faq-add-team-members.md)
