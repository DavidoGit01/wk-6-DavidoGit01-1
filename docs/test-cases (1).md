# 🧪 CleanCity: Test Cases Document  
**Version:** 1.0  
**Date:** 2025-11-13  
**Prepared By:** QA Team  

All test cases below are grouped by module and mapped to requirements from `functional-requirements.md`.  
**Status:** All test cases are currently marked as Executed except 3

---

# 1️⃣ User Authentication (Test Cases 1–10)

| Test Case ID | Requirement ID | Test Scenario | Preconditions | Steps | Expected Result | Status |
|--------------|----------------|---------------|---------------|--------|------------------|---------|
| TC-AUTH-01 | FR-001, FR-002, FR-003 | Successful registration | User not registered | 1. Go to Register 2. Enter valid details 3. Submit | User redirected to login with success message | Executed |
| TC-AUTH-02 | FR-002 | Invalid email format | None | 1. Go to Register 2. Enter invalid email 3. Submit | Error “Invalid email format” | Executed |
| TC-AUTH-03 | FR-002 | Password mismatch | None | 1. Enter password + mismatch confirm 2. Submit | Error “Passwords do not match” | Executed |
| TC-AUTH-04 | FR-002, FR-090 | Password too short | None | 1. Enter short password 2. Submit | Error “Password too short” | Executed |
| TC-AUTH-05 | FR-002 | Existing email | Email already registered | 1. Enter existing email 2. Submit | Error “Email already exists” | Executed |
| TC-AUTH-06 | FR-001 | Name field empty | None | 1. Leave name empty 2. Submit | Error “Name is required” | Executed |
| TC-LOGIN-07 | FR-004 | Successful login | User registered | 1. Enter valid credentials | Redirect to dashboard | Executed |
| TC-LOGIN-08 | FR-005 | Invalid login attempts | User exists | 1. Enter invalid credentials | Error “Invalid credentials” | Executed |
| TC-LOGIN-09 | FR-006 | Session persistence | Logged in user | 1. Login 2. Close browser 3. Reopen | User remains logged in | Executed |
| TC-LOGIN-10 | FR-008 | Logout | Logged in user | Click logout | Redirect to login | Executed |

---

# 2️⃣ Waste Management (Test Cases 11–20)

| Test Case ID | Requirement ID | Test Scenario | Preconditions | Steps | Expected Result | Status |
|--------------|----------------|---------------|---------------|--------|------------------|---------|
| TC-WM-11 | FR-012 | Successful pickup scheduling | User logged in | Fill form correctly | Confirmation + request added | Executed |
| TC-WM-12 | FR-013 | Past date scheduling | User logged in | Choose past date | Error displayed | Executed |
| TC-WM-13 | FR-012, FR-081 | Missing date validation (Bug) | None | Leave date empty | Expected error doesn’t show | Executed |
| TC-WM-14 | FR-013 | Schedule for same day | User logged in | Pick today's date | Error due to 24hr rule | Executed |
| TC-WM-15 | FR-012 | Special instructions > 200 chars | User logged in | Enter >200 chars | Error or truncation | Executed |
| TC-WM-16 | FR-017 | Cancel request | Request exists | Cancel request | Status changed to Cancelled | Executed |
| TC-WM-17 | FR-018 | Modify request | Scheduled request exists | Modify fields | Request updated | Executed |
| TC-WM-18 | FR-018 | Modify < 24hrs | Next-day request exists | Try modifying | Modification blocked | Executd |
| TC-WM-19 | FR-022 | Add feedback | Completed request | Add feedback | Saved | Executed |
| TC-WM-20 | FR-015 | Multiple pickups same day | First request exists | Attempt second | Error displayed | Executed |

---

# 3️⃣ Dashboard & Gamification (Test Cases 21–30)

| Test Case ID | Requirement ID | Scenario | Preconditions | Steps | Expected | Status |
|--------------|----------------|----------|--------------|--------|----------|---------|
| TC-DASH-21 | FR-023 | Dashboard accuracy | User logged in | Open dashboard | Correct pickups displayed | Executed |
| TC-DASH-22 | FR-056 | Location filter (Bug) | Requests exist | Filter table | Eldoret only expected (Bug shows Nairobi) | Executed |
| TC-DASH-23 | FR-024 | Environmental stats | Completed pickups | Open dashboard | Correct stats | Executed |
| TC-DASH-24 | FR-028 | Export data | User logged in | Click export | CSV downloaded | Executed |
| TC-DASH-25 | FR-029 | First pickup badge | First pickup scheduled | Schedule pickup | Badge awarded | Executed |
| TC-DASH-26 | FR-029 | 10 pickups badge | 10 pickups complete | Open dashboard | Badge displayed | Executed |
| TC-DASH-27 | FR-030 | Points system | Perform actions | View points | Points updated | Executed |
| TC-DASH-28 | FR-026 | Leaderboard | Users exist | View leaderboard | Correctly sorted | Executed |
| TC-DASH-29 | FR-038 | Awareness quiz | User logged in | Take quiz | Score tracked | Executed |
| TC-DASH-30 | FR-036 | Eco tips rotation | User logged in | Watch tips | Rotate every 5s | Executed |

---

# 4️⃣ Community & Profile (Test Cases 31–40)

| Test Case | Requirement ID | Scenario | Preconditions | Steps | Expected | Status |
|-----------|----------------|----------|--------------|--------|----------|---------|
| TC-COMM-31 | FR-041 | Create post | User logged in | Create post | Post appears | Executed |
| TC-COMM-32 | FR-042 | Like post | Post exists | Like post | Like++ | Executed |
| TC-COMM-33 | FR-042 | Comment on post | Post exists | Add comment | Comment shown | Executed |
| TC-COMM-34 | FR-041, FR-083 | Empty post blocked | None | Post empty message | Error shown | Executed |
| TC-PROF-35 | FR-045 | Edit profile | Logged in | Edit fields | Save success | Executed |
| TC-PROF-36 | FR-047 | Upload picture | Logged in | Upload image | Image shown | Executed |
| TC-PROF-37 | FR-049 | Follow a user | Another user exists | Click follow | User followed | Executed |
| TC-NOTIF-38 | FR-066 | Notification for like | Another user likes post | Check notifications | Notification appears | Executed |
| TC-NOTIF-39 | FR-067 | Mark notif read | Notification exists | Mark read | Marked | Executed |
| TC-NOTIF-40 | FR-065 | Bell count | Notification received | View bell | Count increases | Executed |

---

# 5️⃣ Admin, UI, A11y & Error Handling (Test Cases 41–50)

| Test Case | Requirement ID | Scenario | Preconditions | Steps | Expected | Status |
|-----------|----------------|----------|--------------|--------|----------|---------|
| TC-ADMIN-41 | FR-054 | Admin UI not refreshing (Bug) | Admin logged in | Update status | Should refresh immediately | Executed |
| TC-ADMIN-42 | FR-061 | Delete post | Admin logged in | Delete | Post removed | Executed |
| TC-ADMIN-43 | FR-058 | Change user role | Admin logged in | Change role | Updated | Executed |
| TC-ADMIN-44 | FR-059 | Suspend user | Admin logged in | Suspend | Cannot log in | Executed |
| TC-UI-45 | FR-069 | Mobile responsive | None | View mobile | Responsive UI | Pending |
| TC-UI-46 | FR-069 | Tablet responsive | None | View tablet | Responsive UI | Pending |
| TC-UI-47 | FR-072 | Keyboard navigation | None | Tab through UI | Logical order | Pending |
| TC-A11Y-48 | FR-073 | Missing alt text (Bug) | Awareness page | Inspect images | Should have alt | Executed |
| TC-A11Y-49 | FR-074 | Screen reader | Screen reader ON | Navigate | Accessible labels | Executed |
| TC-ERROR-50 | FR-087 | User-friendly errors | Trigger errors | View error | Helpful messages | Executed |
