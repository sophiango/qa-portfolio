# Login app — Formal Test Plan

## 1. Overview

**Application Under Test (AUT):** Login app (https://the-internet.herokuapp.com/login) is a simple login web application allowing users to log in using username + password

### Purpose of Testing

The goal of this test effort is to verify that Login web app can perform some validations when user performs login action

---

## 2. Objectives & Success Criteria

### Objectives

- Validate functional behavior against expected requirements  
- Identify and isolate defects early  
- Ensure critical workflows operate reliably  
- Confirm UI state reflects underlying data accurately  

### Success Criteria

Testing is considered successful when:

- All **P0 and P1 defects are resolved or mitigated**
- All defined **test cases are executed**
- Defined acceptance criteria pass

---

## 3. In-Scope Testing

The following areas are included:

- Valid login
- Invalid login
- Empty fields
- Security messaging
- UI behavior 

---

## 4. Out-of-Scope Testing

The following are excluded for this test cycle:

- Backend API validation
- Performance testing
- Rate limits

These may be included in future phases.

---

## 5. Risks & Assumptions

- Users may accidentally enter wrong password
- Users may try blank fields
- Browser refresh must preserve state (confirm)
- Login error messages must NOT expose sensitive details

---

## 6. Test Environment

OS: macOS Sequoia
Browser: Safari latest
Network: stable wifi

### Test Data

Valid username: tomsmith
Valid password: SuperSecretPassword!
Invalid password: wrongpass
Invalid username: abc123

### Build / Version
- Public Login app implementation