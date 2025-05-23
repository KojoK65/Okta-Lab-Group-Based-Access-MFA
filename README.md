# Okta Lab: Group-Based Access + MFA

This lab demonstrates core IAM administration tasks using Okta — including user creation, group-based access control, SAML app configuration, and MFA enforcement. The setup was completed within the Okta Admin Console.
---

## ✅ Step-by-Step Lab Workflow

## 🔹 Step 1: Created Test Users
Created two users to simulate employees in different departments:
- `testuser1@Flexpunch.com`
- `testuser2@Flexpunch.com`

<img width="1280" alt="Screen Shot 2025-05-23 at 3 44 06 PM" src="https://github.com/user-attachments/assets/37216b23-85b5-40d7-98f4-4912cd27c494" />

---

## 🔹 Step 2: Created Two User Groups
Created `Engineering` and `Sales` groups to simulate organizational roles.

<img width="1280" alt="Screen Shot 2025-05-23 at 3 51 15 PM" src="https://github.com/user-attachments/assets/c3190eae-0fd2-49c1-904f-57b8302fd842" />

---

## 🔹 Step 3: Assigned Users to Groups
Assigned:
- `testuser1` to the **Engineering** group

<img width="1280" alt="Screen Shot 2025-05-23 at 3 51 02 PM" src="https://github.com/user-attachments/assets/67854914-3658-4555-b6f5-71cbc07d4d4f" />

- `testuser2` to the **Sales** group

<img width="1280" alt="Screen Shot 2025-05-23 at 3 47 40 PM" src="https://github.com/user-attachments/assets/cb227d41-c0d7-46e3-babf-8269d4454027" />

---

## 🔹 Step 4: Created a Simulated SAML App
Created an app called **Finance Portal** using SAML 2.0 to simulate a protected enterprise application.

<img width="1280" alt="Screen Shot 2025-05-23 at 3 56 49 PM" src="https://github.com/user-attachments/assets/2ee889a8-2add-4087-8fc5-1befbb9da418" />

---

## 🔹 Step 5: Configured SAML Settings
Entered simulated values for SAML settings:
- SSO URL: `https://example.com/sso/acs`
- Entity ID: `https://example.com/sp`

<img width="1280" alt="Screen Shot 2025-05-23 at 3 53 45 PM" src="https://github.com/user-attachments/assets/e85f484b-7830-4022-b958-bff4dfe6d740" />

---

## 🔹 Step 6: Assigned App to the Engineering Group
Granted access to the Finance Portal app only to the Engineering group.

<img width="1280" alt="Screen Shot 2025-05-23 at 3 57 42 PM" src="https://github.com/user-attachments/assets/e56b55ec-c8f6-41a7-bfc2-65a6cea0eef6" />

---

### 🔹 Step 7: Created MFA Authentication Policy
Created an MFA policy requiring password + another factor (e.g., Okta Verify) for app access.

<img width="1280" alt="Screen Shot 2025-05-23 at 4 10 58 PM" src="https://github.com/user-attachments/assets/44f99a42-3d88-4716-9510-33d120dfe209" />

---

### 🔹 Step 8: Attached Policy to the App
Linked the MFA policy to the Finance Portal app to enforce stronger authentication.

<img width="1280" alt="Screen Shot 2025-05-23 at 4 24 18 PM" src="https://github.com/user-attachments/assets/d61d379e-c7a0-4a4a-b7de-98282f6e80c1" />

---

## 🧠 IAM Concepts Demonstrated

| Concept | Demonstrated |
|---------|--------------|
| User and group management | ✅ |
| Group-based access control | ✅ |
| App assignment via groups | ✅ |
| SAML app configuration | ✅ |
| MFA enforcement through policy | ✅ |
| Least privilege access model | ✅ |
