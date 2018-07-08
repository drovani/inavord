# inavord

Starter template for C# CQRS on Azure projects

## Roadmap For Success

- [x] Determine how to store secrets/passwords/connection strings in Open Source Code
  - [ ] Write a blog post about it
- [x] Create mini proof-of-concept projects throughout solution to demonstrate the viability of each idea

## Authentication

[Azure Active Directory B2C](https://azure.microsoft.com/en-us/services/active-directory-b2c/) provides the authentication mechanism.

- 

### Future Authentication Goals

- [x] Ability to plug into Azure Active Directory B2C
- [ ] Ability to connect to any OAuth2 authenticator
- [ ] Ability to authenticate with different providers and segregate users based on login (i.e. internal users through AAD, external users through AAD B2C  or Facebook or Twitter)

## Authorization

Roll based authorizations, starting with hard-coded list of groups:

- [ ] Administrator (can do anything)
- [ ] Power User (can override most non-system-breaking business rules)
- [ ] Case Manager (user that can view sensitive information on select accounts)
- [ ] Standard User (internal employee doing most day-to-day work)
- [ ] Restricted User (external vendor restricted to less sensitive information)
- [ ] User Account (login tied to a single Patron and restricted to only viewing that information)

### Future Authorization Goals

- [ ] Fully customizable roles and privilege assignments
- [ ] Privilege assignments to granular levels (perhaps even as far as field level read/write)
