

# Day 10 - Creating a Conditional Access Policy: Block legacy authentication

## Introduction

Due to the increased risk associated with legacy authentication protocols, Microsoft recommends that organizations block authentication requests using these protocols and require modern authentication.




###  Create a Conditional Access policy

The following steps will help create a Conditional Access policy to block legacy authentication requests. This policy is put in to Report-only mode to start so administrators can determine the impact they will have on existing users. When administrators are comfortable that the policy applies as they intend, they can switch to On or stage the deployment by adding specific groups and excluding others.

1) Sign in to the Azure portal as a global administrator, security administrator, or Conditional Access administrator.

2) Browse to Azure Active Directory > Security > Conditional Access.
3) Select New policy.
4) Give your policy a name. We recommend that organizations create a meaningful standard for the names of their policies.
5) Under Assignments, select Users and groups
a) Under Include, select All users.
b) Under Exclude, select Users and groups and choose any accounts that must maintain the ability to use legacy authentication. Exclude at least one account to prevent yourself from being locked out. If you do not exclude any account, you will not be able to create this policy.
c) Select Done.
6) Under Cloud apps or actions, select All cloud apps.
a) Select Done.
7) Under Conditions > Client apps, set Configure to Yes.
a) Check only the boxes Exchange ActiveSync clients and Other clients.
b) Select Done.
8) Under Access controls > Grant, select Block access.
a) Select Select.
9) Confirm your settings and set Enable policy to Report-only.
10) Select Create to create to enable your policy.

After confirming your settings using report-only mode, an administrator can move the Enable policy toggle from Report-only to On.
