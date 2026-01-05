# 🧪 ToDoMVC — Formal Test Plan

## 1. Overview

**Application Under Test (AUT):** ToDoMVC (https://todomvc.com/examples/react/dist/#/) — a simple task-tracking web application that allows users to create and manage todo items.

### Purpose of Testing

The goal of this test effort is to verify that ToDoMVC:

- Correctly supports creating, editing, completing, deleting, and filtering todos
- Preserves data integrity and expected state across interactions
- Provides a consistent, usable experience across core flows
- Handles invalid or unexpected input gracefully

This test plan defines the scope, strategy, objectives, resources, risks, and schedule for validation.

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

- Adding todos  
- Editing todos  
- Marking todos completed/active  
- Deleting todos  
- Filter functionality  
- Counter behavior  
- Toggle All behavior  
- Clearing completed  
- Input validation  
- Basic UI state (labels, completion styling, counts)  

---

## 4. Out-of-Scope Testing

The following are excluded for this test cycle:

- Performance benchmarking  
- Browser compatibility outside Chrome  
- Accessibility audit  
- API testing  
- Security testing  
- Mobile-specific UI  

These may be included in future phases.

---

## 5. Assumptions

- User starts with a working browser (Chrome latest)
- App loads successfully
- Network connectivity is available
- No authentication is required

---

## 6. Test Environment

OS: macOS Sequoia
Browser: Safari latest
Network: stable wifi

### Test Data
Example todo inputs:

- `Buy milk`
- `Learn QA`
- `Walk the dog`

### Build / Version
- Public ToDoMVC implementation