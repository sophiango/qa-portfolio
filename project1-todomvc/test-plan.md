# 🧪 ToDoMVC — Formal Test Plan

## 1. Overview

**Application Under Test (AUT):** ToDoMVC — a simple task-tracking web application that allows users to create and manage todo items.

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

### Hardware / OS
- macOS or Windows laptop

### Browser
- Google Chrome (latest)

### Test Data
Example todo inputs:

- `Buy milk`
- `Learn QA`
- `Walk the dog`

### Build / Version
- Public ToDoMVC implementation  
  *(or specify your hosted version if applicable)*

---

## 7. Test Strategy & Types of Testing

### 7.1 Functional Testing
- Positive & negative scenarios  
- CRUD operations  
- UI behavior validation  

### 7.2 Exploratory Testing
- Edge cases  
- Unusual user behavior  
- Rapid interaction patterns  

### 7.3 Regression Testing
- Re-execution of critical flows after defect fixes  

---

## 8. Test Case Summary

| ID | Title | Priority |
|---|---|---|
| TC-001 | Add a Single Todo Item | P0 |
| TC-002 | Add Multiple Todo Items | P0 |
| TC-003 | Prevent Adding Empty Todo | P1 |
| TC-004 | Trim Leading and Trailing Spaces | P2 |
| TC-005 | Mark a Todo as Completed | P0 |
| TC-006 | Uncheck a Completed Todo | P0 |
| TC-007 | Edit an Existing Todo | P1 |
| TC-008 | Cancel Edit Without Saving | P2 |
| TC-009 | Delete a Todo Item | P0 |
| TC-010 | Toggle All to Complete | P1 |
| TC-011 | Toggle All to Active | P1 |
| TC-012 | Filter to Show Only Active | P1 |
| TC-013 | Filter to Show Only Completed | P1 |
| TC-014 | Clear Completed Items | P0 |
| TC-015 | Todo Counter Updates Correctly | P1 |

> Full details available in: `todomvc_test_cases.csv`

---

## 9. Exit Criteria

Testing is complete when:

- 100% of planned test cases are executed  
- 100% of **P0/P1 defects are fixed or formally deferred**  
- Test results are documented  
- No outstanding blocking issues remain  

---

## 10. Risk Assessment

### High Risk
- Loss of todos due to delete/clear bugs  
- Incorrect save/edit state  

### Medium Risk
- Filters showing incorrect data  

### Low Risk
- UI polish issues  

**Mitigation:** perform regression runs after each fix.

---

## 11. Defect Tracking

Each defect will include:

- Title  
- Steps to Reproduce  
- Expected Result  
- Actual Result  
- Severity  
- Priority  
- Environment  
- Screenshots (if possible)  

### Severity Levels

- **S1 — Critical (app unusable)**
- **S2 — Major**
- **S3 — Minor**
- **S4 — Cosmetic**

---

## 12. Reporting

Daily QA update includes:

- Test execution progress
- Number of defects opened / closed
- Risks / blockers
- Summary of key findings

---

## 13. Roles & Responsibilities

### QA Engineer — **Sophia Ngo**

- Create test plan & test cases  
- Execute tests  
- Log defects  
- Provide QA reporting  

*(Optional to include other roles)*

---

## 14. Tools

- Safari 
- GitHub (documentation + test artifacts)

---

## 15. Acceptance Criteria

The build is acceptable when:

- All **P0/P1 defects are resolved or formally waived**
- Critical workflows are stable  
- There is no data corruption  

