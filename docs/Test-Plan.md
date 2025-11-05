# 🧾 CleanCity Application – Test Plan & Strategy Document

## 1. Project Overview
**Project Name:** CleanCity - Waste Pickup Scheduler  
**Version:** v1.0  
**Prepared By:** Madumere David  
**Date:** 5/11/2025

### 1.1 Purpose
This Test Plan outlines the overall strategy and approach for testing the CleanCity web application. It ensures that all functional and non-functional requirements are validated before final delivery.

### 1.2 Application Summary
The **CleanCity App** is designed to promote environmental cleanliness and community reporting.  
Users can:
- Report waste or pollution in their area  
- Track cleanup requests  
- View community initiatives  
- Get updates and rewards for eco-friendly participation  

---

## 2. Test Objectives
- Verify that all application features work as intended.  
- Detect defects early and ensure they are resolved before release.  
- Validate that the app meets both functional and non-functional requirements.  
- Ensure the system is user-friendly, reliable, and performs efficiently.

---

## 3. Scope of Testing

### 3.1 In Scope
- Functional testing of all modules (Authentication, Scheduling, Dashboard, etc.).  
- Non-functional testing including usability, performance, and accessibility.  
- Cross-browser and device compatibility testing.  


### 3.2 Out of Scope
- Backend and API testing (no backend available).  
- Extensive security penetration testing. 

---

## 4. Test Strategy

### 4.1 Testing Levels
| Level | Description |
|--------|--------------|
| **Unit Testing** | Performed by developers. |
| **Integration Testing** | Validation between modules like scheduling and dashboard. |
| **System Testing** | End-to-end testing on all functionalities. |
| **Regression Testing** | Re-running previous tests after fixes. |
| **Acceptance Testing** | Final review and sign-off by QA team. |

### 4.2 Testing Types
| Type | Objective |
|-------|------------|
| **Functional Testing** | Ensure app features perform according to requirements |
| **UI/UX Testing** | Verify interface consistency and user navigation flow |
| **Cross-browser Testing** | Test on Chrome, Edge, and Firefox |
| **Responsive Testing** | Check mobile, tablet, and desktop compatibility |
| **Smoke Testing** | Quick check after new build deployment |
| **Regression Testing** | Recheck after bug fixes and updates |

### 4.3 Test Approach
Testing will be **manual**, following systematic test case design and execution. Defects will be tracked using **GitHub Issues **, linked to test cases and progress updates.
---

## 5. Test Deliverables
| Deliverable | Description |
|--------------|-------------|
| Test Plan Document | Overall strategy and scope (this document) |
| Test Scenarios & Test Cases | Detailed steps and expected results |
| Test Data | Sample input data used for validation |
| Defect Reports | Logged bugs and their resolutions |
| Test Summary Report | Final evaluation of testing activities |

---

## 6. Test Environment
| Component | Details |
|------------|----------|
| Environment | Details |
|--------------|----------|
| **Platform** | Web application hosted on Netlify |
| **Browsers** | Chrome, Edge, Firefox, Safari |
| **Devices** | Desktop, Tablet, Mobile |
| **Tools** | GitHub Projects (Kanban) |


---

## 7. Entry and Exit Criteria
| Criteria Type | Description |
|----------------|--------------|
| **Entry** | Requirements approved, build deployed, test data ready. |
| **Exit** | All planned tests executed, critical bugs fixed, summary report completed. |

---

## 8. Test Schedule (Example)
| Phase | Task | Duration | Owner |
|--------|------|-----------|--------|
| Planning | Define objectives, scope, and resources | 2 days | Test Manager |
| Design | Write test cases and scenarios | 2 days | Risk analyst |
| Execution | Run tests and log defects | 4 days | QA Testers |
| Reporting | Prepare summary and metrics | 2 days | Test Manager |
---

## 9. Roles and Responsibilities
Role	|Name	|Responsibilities
Team Lead |David Madumere |	Oversees testing process and ensures deadlines
Test Analyst|Samuel Ezereonye|	Designs test cases and prepares test data
Tester |Oghenerume Igbriwi| Executes manual test cases
Tester |Oghenerume Igbriwi |Validates bug fixes and retesting
Documentation Lead |David Madumere| Prepares Test Plan & Bug Reports

---

## 10. Risk & Mitigation Plan
| Risk | Impact | Mitigation |
|------|---------|-------------|
| Limited time for testing | High | Prioritize high-risk modules. |
| Environment unavailability | Medium | Use backup local version. |
| Incomplete requirements | High | Communicate promptly with stakeholders. |
| Frequent changes | Medium | Re-run regression tests after each change. |

---

## 11. Defect Management Process
**Tool Used:** GitHub Issues  

Each defect will include:
- Issue Title  
- Steps to Reproduce  
- Expected vs Actual Result  
- Screenshots (if applicable)  
- Severity: `Low | Medium | High | Critical`  
- Status: `New → In Progress → Fixed → Retested → Closed`

---

## 12. Metrics and Reporting
| Metric | Description |
|----------|--------------|
| Test Case Execution Rate | Percentage of executed vs planned test cases. |
| Defect Density | Number of defects per module. |
| Defect Fix Rate | Percentage of defects resolved. |
| Test Coverage | Percentage of functionalities tested. |
| Pass/Fail Rate | Test case success ratio. |

---

##  13. Test Closure
At the end of testing, the QA team will:
- Review defect resolution status.  
- Summarize test coverage and metrics.  
- Document lessons learned.  
- Submit a final test report and presentation video. 
---

## 14. Approval
| Name | Role | Signature | Date |
|-------|-------|------------|------|
| Madumere David | Test Manager |  |  |
| [Supervisor Name] | QA Supervisor |  |  |
