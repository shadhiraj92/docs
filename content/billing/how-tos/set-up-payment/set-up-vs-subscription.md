---
title: Setting up Visual Studio subscriptions with GitHub Enterprise
intro: 'Your team''s subscription to {% data variables.product.prodname_vs %} can also provide access to {% data variables.product.prodname_enterprise %}.'
versions:
  ghec: '*'
redirect_from:
  - /billing/managing-licenses-for-visual-studio-subscriptions-with-github-enterprise/setting-up-visual-studio-subscriptions-with-github-enterprise
  - /billing/managing-billing-for-your-products/managing-licenses-for-visual-studio-subscriptions-with-github-enterprise/setting-up-visual-studio-subscriptions-with-github-enterprise
  - /billing/managing-licenses-for-visual-studio-subscriptions-with-github-enterprise
  - /billing/managing-billing-for-your-products/managing-licenses-for-visual-studio-subscriptions-with-github-enterprise
topics:
  - Billing
  - Enterprise
  - Licensing
shortTitle: Set up VS subscription
contentType: how-tos
---

## About setup of {% data variables.visual_studio.prodname_vss_ghe %}

{% data reusables.enterprise-accounts.vss-ghe-description %} See [AUTOTITLE](/billing/managing-billing-for-your-products/managing-licenses-for-visual-studio-subscriptions-with-github-enterprise/about-visual-studio-subscriptions-with-github-enterprise).

This guide shows you how your team can get {% data variables.product.prodname_vs %} subscribers licensed and started with {% data variables.product.prodname_enterprise %}.

## Roles for {% data variables.visual_studio.prodname_vss_ghe %}

Before setting up {% data variables.visual_studio.prodname_vss_ghe %}, it's important to understand the roles for this combined offering.

| Role | Service | Description | More information |
| :- | :- | :- | :- |
| **Subscriptions admin** | {% data variables.product.prodname_vs %} subscription | Person who assigns licenses for {% data variables.product.prodname_vs %} subscription | [Overview of admin responsibilities](https://docs.microsoft.com/en-us/visualstudio/subscriptions/admin-responsibilities) in Microsoft Docs |
| **Subscriber** | {% data variables.product.prodname_vs %} subscription | Person who uses a license for {% data variables.product.prodname_vs %} subscription | [Visual Studio Subscriptions documentation](https://docs.microsoft.com/en-us/visualstudio/subscriptions/) in Microsoft Docs |
| **Enterprise owner** | {% data variables.product.prodname_dotcom %} | Person who has a personal account that's an administrator of an enterprise on {% data variables.location.product_location %} | [AUTOTITLE](/admin/user-management/managing-users-in-your-enterprise/roles-in-an-enterprise#enterprise-owner) |
| **Organization owner** | {% data variables.product.prodname_dotcom %} | Person who has a personal account that's an owner of an organization in your team's enterprise on {% data variables.location.product_location %} | [AUTOTITLE](/organizations/managing-peoples-access-to-your-organization-with-roles/roles-in-an-organization#organization-owners) |
| **Enterprise member** | {% data variables.product.prodname_dotcom %} | Person who has a personal account that's a member of an enterprise on {% data variables.location.product_location %} | [AUTOTITLE](/admin/user-management/managing-users-in-your-enterprise/roles-in-an-enterprise#enterprise-members)  |

## Prerequisites

* Your team's {% data variables.product.prodname_vs %} subscription must include {% data variables.product.prodname_enterprise %}. For more information, see [{% data variables.product.prodname_vs %} Subscriptions and Benefits](https://visualstudio.microsoft.com/subscriptions/) on the {% data variables.product.prodname_vs %} website and [Overview of admin responsibilities](https://docs.microsoft.com/en-us/visualstudio/subscriptions/admin-responsibilities) in Microsoft Docs.

* Your team must have an enterprise on {% data variables.location.product_location %}. If you're not sure whether your team has an enterprise, contact your {% data variables.product.prodname_dotcom %} administrator. If you're not sure who on your team is responsible for {% data variables.product.prodname_dotcom %}, contact {% data variables.contact.contact_enterprise_sales %}. For more information, see [AUTOTITLE](/admin/overview/about-enterprise-accounts).

## Setting up {% data variables.visual_studio.prodname_vss_ghe %}

To set up {% data variables.visual_studio.prodname_vss_ghe %}, members of your team must complete the following tasks.

One person may be able to complete the tasks because the person has all of the roles, but you may need to coordinate the tasks with multiple people. For more information, see [Roles for {% data variables.visual_studio.prodname_vss_ghe %}](#roles-for-visual-studio-subscriptions-with-github-enterprise).

1. An enterprise owner must create at least one organization in your enterprise on {% data variables.location.product_location %}. For more information, see [AUTOTITLE](/admin/user-management/managing-organizations-in-your-enterprise/adding-organizations-to-your-enterprise).

1. The subscription admin must assign a license for {% data variables.product.prodname_vs %} to a subscriber in {% data variables.visual_studio.prodname_vss_admin_portal_with_url %}. For more information, see [Overview of the {% data variables.product.prodname_vs %} Subscriptions Administrator Portal](https://docs.microsoft.com/en-us/visualstudio/subscriptions/using-admin-portal) and [Assign {% data variables.product.prodname_vs %} Licenses in the {% data variables.product.prodname_vs %} Subscriptions Administration Portal](https://docs.microsoft.com/en-us/visualstudio/subscriptions/assign-license) in Microsoft Docs.

1. Optionally, if the subscription admin assigned licenses to subscribers in {% data variables.product.prodname_vs %} before adding {% data variables.product.prodname_enterprise %} to the subscription, the subscription admin can move the subscribers to the combined offering in the {% data variables.product.prodname_vs %} administration portal. For more information, see [Manage {% data variables.product.prodname_vs %} subscriptions with {% data variables.product.prodname_enterprise %}](https://docs.microsoft.com/en-us/visualstudio/subscriptions/assign-github#moving-to-visual-studio-with-github-enterprise) in Microsoft Docs.

1. If the subscription admin has not disabled email notifications, the subscriber will receive two confirmation emails. For more information, see [{% data variables.product.prodname_vs %} subscriptions with {% data variables.product.prodname_enterprise %}](https://docs.microsoft.com/en-us/visualstudio/subscriptions/access-github#what-is-the-visual-studio-subscription-with-github-enterprise-setup-process) in Microsoft Docs.

1. An organization owner must invite the subscriber to the organization on {% data variables.location.product_location %} from step 1. The subscriber can accept the invitation with an existing personal account or create a new account. After the subscriber joins the organization, the subscriber becomes an enterprise member. For more information, see [AUTOTITLE](/organizations/managing-membership-in-your-organization/inviting-users-to-join-your-organization).

   > [!TIP]
   > * While not required, we recommend that the organization owner sends an invitation to the same email address used for the subscriber's User Primary Name (UPN). When the email address on {% data variables.location.product_location %} matches the subscriber's UPN, you can ensure that another enterprise does not claim the subscriber's license.
   > * If the subscriber accepts the invitation to the organization with an existing personal account on {% data variables.location.product_location %}, we recommend that the subscriber add the email address they use for {% data variables.product.prodname_vs %} to their personal account on {% data variables.location.product_location %}. For more information, see [AUTOTITLE](/account-and-profile/setting-up-and-managing-your-personal-account-on-github/managing-email-preferences/adding-an-email-address-to-your-github-account).
   > * If the organization owner must invite a large number of subscribers, a script may make the process faster. For more information, see [the sample PowerShell script](https://github.com/github/platform-samples/blob/master/api/powershell/invite_members_to_org.ps1) in the `github/platform-samples` repository.

1. If any enterprise members aren't automatically matched to their {% data variables.product.prodname_vs %} account, an enterprise owner can match the accounts manually on {% data variables.product.github %}. See [Reconciling users across {% data variables.product.prodname_vs %} and {% data variables.product.github %}](#reconciling-users-across-visual-studio-and-github).

After {% data variables.visual_studio.prodname_vss_ghe %} is set up for subscribers on your team, enterprise owners can review licensing information on {% data variables.location.product_location %}. For more information, see [AUTOTITLE](/billing/managing-the-plan-for-your-github-account/viewing-the-subscription-and-usage-for-your-enterprise-account).

## Reconciling users across {% data variables.product.prodname_vs %} and {% data variables.product.github %}

To stay compliant with the terms of use, a {% data variables.product.github %} **enterprise owner** should ensure all user accounts are correctly matched across {% data variables.product.github %} and {% data variables.product.prodname_vs %}.

Most users are automatically matched across {% data variables.product.github %} and {% data variables.product.prodname_vs %}. If a user has different email addresses in {% data variables.product.github %} and {% data variables.product.prodname_vs %}, you may need to match the accounts manually.

Under the terms of use, the {% data variables.product.github %} account and {% data variables.product.prodname_vs %} account for a single license must belong to the same person.

### 1. Audit user mappings

To audit your user mappings, download a summary of assigned users from the {% data variables.product.prodname_vs %} portal, and compare it against the verified emails of users in your {% data variables.product.github %} enterprise. See [AUTOTITLE](/enterprise-cloud@latest/admin/managing-accounts-and-repositories/managing-users-in-your-enterprise/viewing-people-in-your-enterprise#viewing-members-email-addresses).

### 2. Match users to {% data variables.product.prodname_vs %}

When you've identified {% data variables.product.github %} users who aren't correctly matched to their {% data variables.product.prodname_vs %} account, you can update the mappings on {% data variables.product.github %}. You can't update mappings for users who have been automatically matched.

1. Go to your enterprise on {% data variables.product.github %} and click **{% octicon "credit-card" aria-hidden="true" aria-label="credit-card" %} Billing and licensing**.
1. In the left sidebar, click **{% octicon "law" aria-hidden="true" aria-label="law" %} Licensing**.
1. On the Licensing page, next to "Enterprise Cloud", click **Manage**.
1. In the list of users, look for users with an "Enterprise" license type. These are enterprise members that aren't matched to a user in your {% data variables.product.prodname_vs %} subscription.
1. To match a user to their {% data variables.product.prodname_vs %} account, click {% octicon "kebab-horizontal" aria-label="More options" %}, then click **Change to {% data variables.product.prodname_vs %} license**.
1. Select the user's {% data variables.product.prodname_vs %} login email, then click **Confirm change**.

## Further reading

* [AUTOTITLE](/get-started/onboarding/getting-started-with-github-enterprise-cloud)
