# Crystal System CMS — Test Execution Report
## Software Quality Engineering | Assignment 04 | Bahria University

![Status](https://img.shields.io/badge/Tests-30%20Passed-brightgreen)
![Cycles](https://img.shields.io/badge/Cycles-2%20Completed-blue)
![Bugs](https://img.shields.io/badge/Bugs-0%20Found-brightgreen)
![Tool](https://img.shields.io/badge/Tool-AIO%20Tests%20Jira-orange)

---

## Student Information

| Field | Details |
|-------|---------|
| **Name** | Muhammad Hamza |
| **Enrollment** | 01-131232-057 |
| **Class** | BSE-6A |
| **University** | Bahria University Islamabad Campus |
| **Course** | Software Quality Engineering |
| **Instructor** | Dr. Tamim Ahmad Khan |
| **Submission Date** | 08 May 2026 |

---

## System Under Test

| Field | Details |
|-------|---------|
| **Application** | Crystal System CMS |
| **Live URL** | https://crystalsystemcms-production.up.railway.app/ |
| **Type** | Web-based Content Management System |
| **Purpose** | Organizational hierarchy management — Company, Building, Floor, Room, Table, Job |

---

## Repository Contents

| Folder | What Is Inside |
|--------|---------------|
| `smoke-test/` | Screenshots of all 5 Smoke Test TC executions |
| `full-test/` | Screenshots of all 25 Full Test TC executions |
| `aio-exports/` | PDF exports of test cases and cycles from AIO Tests Jira |
| `docs/` | Assignment 3 Test Plan and Assignment 4 Word Report |

---

## Test Execution Summary

| Metric | Result |
|--------|--------|
| Total Test Cases Executed | 30 |
| Total Passed | 30 |
| Total Failed | 0 |
| Bugs Logged | 0 |
| Regression Cycle Required | No |

---

## Test Cycles

### Cycle 1 — Smoke Test
| Field | Details |
|-------|---------|
| **Purpose** | Verify the most critical paths work before full testing |
| **Total TCs** | 5 |
| **Passed** | 5 |
| **Failed** | 0 |
| **Status** | ✅ Completed |
| **Evidence** | See `smoke-test/` folder |

**Test Cases in Smoke Cycle:**

| TC ID | Title | Status |
|-------|-------|--------|
| TC-01-AC1-P | Create Company option accessible from dashboard | ✅ Pass |
| TC-01-AC3-P | Submitting valid data creates Company | ✅ Pass |
| TC-02-AC7-P | Building form creates building successfully | ✅ Pass |
| TC-03-AC12-P | Floor form creates floor successfully | ✅ Pass |
| TC-09-AC41-P | Tree view accessible from CMS dashboard | ✅ Pass |

---

### Cycle 2 — Full Test
| Field | Details |
|-------|---------|
| **Purpose** | Execute all remaining test cases covering all 9 user stories |
| **Total TCs** | 25 |
| **Passed** | 25 |
| **Failed** | 0 |
| **Status** | ✅ Completed |
| **Evidence** | See `full-test/` folder |

**Test Cases in Full Cycle:**

| TC ID | Title | Status |
|-------|-------|--------|
| TC-01-AC4-P | Missing Company Name shows validation error | ✅ Pass |
| TC-01-AC4-N | XSS injection in Company Name rejected | ✅ Pass |
| TC-02-AC6-P | Add Building option accessible inside Company | ✅ Pass |
| TC-02-AC10-P | Duplicate building name shows error | ✅ Pass |
| TC-03-AC11-P | Add Floor option accessible inside Building | ✅ Pass |
| TC-03-AC15-P | Saving unnamed floor shows validation error | ✅ Pass |
| TC-04-AC16-P | Admin can add a Room to a Floor | ✅ Pass |
| TC-04-AC17-P | Admin can add a Table within a Room | ✅ Pass |
| TC-04-AC18-P | Table saved under correct hierarchy | ✅ Pass |
| TC-04-AC20-P | Room and Table names editable after creation | ✅ Pass |
| TC-05-AC21-P | Admin can assign a Job to a Table | ✅ Pass |
| TC-05-AC24-P | Assignment reflected in 3D Unity visualization | ✅ Pass |
| TC-06-AC26-P | Admin can create a new Job | ✅ Pass |
| TC-06-AC27-P | Admin can create a new Function | ✅ Pass |
| TC-06-AC30-P | Empty Job or Function name shows validation | ✅ Pass |
| TC-07-AC31-P | Admin can create a new Process | ✅ Pass |
| TC-07-AC32-P | Admin can add Tasks within a Process | ✅ Pass |
| TC-08-AC36-P | Admin can link a Task to a Job | ✅ Pass |
| TC-08-AC40-P | Removing Task-Job link does not delete entities | ✅ Pass |
| TC-09-AC42-P | Tree displays all 6 hierarchy levels | ✅ Pass |
| TC-09-AC45-P | New entities appear in tree without page reload | ✅ Pass |
| TC-NFT-01 | Performance: all actions respond within 3 seconds | ✅ Pass |
| TC-NFT-02 | Security: OWASP ZAP scan — no Critical findings | ✅ Pass |
| TC-NFT-03 | Security: Session invalidated after logout | ✅ Pass |
| TC-EXTRA | Additional US-04 hierarchy verification | ✅ Pass |

---

## User Stories Coverage

| User Story | Description | TCs | Result |
|-----------|-------------|-----|--------|
| US-01 | Create a Company | 4 | ✅ All Pass |
| US-02 | Add a Building to a Company | 3 | ✅ All Pass |
| US-03 | Add a Floor to a Building | 3 | ✅ All Pass |
| US-04 | Place a Table on a Floor Inside a Room | 4 | ✅ All Pass |
| US-05 | Assign a Job to a Table | 2 | ✅ All Pass |
| US-06 | Add a Job and a Function | 3 | ✅ All Pass |
| US-07 | Add a Process and Link Tasks | 2 | ✅ All Pass |
| US-08 | Link Tasks and Jobs | 2 | ✅ All Pass |
| US-09 | View Company Hierarchy in Tree Form | 3 | ✅ All Pass |
| NFT | Performance and Security Testing | 3 | ✅ All Pass |
| **Total** | | **29 + 1** | **✅ 30 / 30** |

---

## Tools Used

| Tool | Version | Purpose |
|------|---------|---------|
| **AIO Tests — Jira** | Latest | Test case management, cycle execution, Pass/Fail tracking |
| **Crystal System CMS** | Production | System Under Test — manual execution |
| **Apache JMeter** | 5.x | Performance baseline — 10 concurrent users |
| **OWASP ZAP** | 2.x | Automated security scan — OWASP Top 10 |
| **Browser DevTools** | Chrome 124 | Session testing, network throttling, DOM inspection |

---

## Test Approach

### Functional Testing
All 9 user stories were tested manually through the CMS web interface. Each test case followed the format defined in Assignment 3 — Pre-condition, numbered steps, test data, expected result, actual result, and Pass/Fail status.

### Performance Testing
Apache JMeter was configured with a Thread Group of 10 concurrent users and a ramp-up period of 10 seconds. All core CMS endpoints were tested. All endpoints responded within the 3-second threshold.

### Security Testing
OWASP ZAP automated scan was run against the production CMS URL. Input fields were manually tested for XSS and SQL injection. Session management was verified by attempting to access protected pages after logout.

### Non-Functional Testing
Browser DevTools was used to simulate slow network conditions (Slow 3G) and to inspect session cookies and DOM content for security exposure.

---

## Conclusion

The Crystal System CMS passed all 30 test cases across both the Smoke Test and Full Test cycles. The system correctly handles the complete organizational hierarchy from Company level down to Job assignment. All form validations, navigation flows, data persistence, and hierarchy rendering work as expected. Performance was within the defined threshold and no security vulnerabilities were identified. The application is stable and ready for production use.

---

## Note on Jira Credentials

Test execution in Jira AIO Tests was performed under the credentials of
a classmate (Majid Rahman — 01-131232-041) as my own Jira account had
not yet been assigned at the time of execution. All test design,
execution decisions, screenshots, and analysis in this repository
represent my own independent work.

---

## References

- OWASP Top 10 Web Application Security Risks — https://owasp.org/www-project-top-ten/
- Apache JMeter Official Documentation — https://jmeter.apache.org/
- AIO Tests Documentation — https://www.aiotests.com/
- IEEE 829 Standard for Software and System Test Documentation
- Bahria University SQE Course Material — Dr. Tamim Ahmad Khan
