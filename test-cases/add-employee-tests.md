# Test Suite: Employee Management – Test Cases

##  Type: Smoke & Sanity  
##  Preconditions (for all): HR user is logged in and is on the correct page (Employees or Settings)

---

### Test Case C1: Adding a new employee with valid input data

**Priority:** High  
**Type:** Smoke & Sanity  

**Steps and Expected Results:**

| Step | Action | Expected Result |
|------|--------|-----------------|
| 1 | Click "Add Employee" button | "Create Employee" form opens |
| 2 | Enter "Maja" into the Name field | Name is entered without validation error |
| 3 | Enter "Nikolic" into the Surname field | Surname is entered without validation error |
| 4 | Enter "majanikolic39@gmail.com" into the Email field | Email is entered and format is validated |
| 5 | Select "Beograd" from the Location dropdown | Location is selected successfully |
| 6 | Select "200-tokena" from the Tier dropdown | Tier is selected successfully |
| 7 | Click "Add" button | User is returned to Employees page, success message: "Employee successfully added!" appears, and new employee is listed |

---

### Test Case C2: Verify that new employee cannot be added without email data

**Priority:** High  
**Type:** Smoke & Sanity  

**Steps and Expected Results:**

| Step | Action | Expected Result |
|------|--------|-----------------|
| 1 | Click "Add Employee" button | "Create Employee" form opens |
| 2 | Enter "Maja" into the Name field | Name is entered without validation error |
| 3 | Enter "Nikolic" into the Surname field | Surname is entered without validation error |
| 4 | Leave the Email field empty | No input in email field |
| 5 | Select "Beograd" from the Location dropdown | Location is selected successfully |
| 6 | Select "200-tokena" from the Tier dropdown | Tier is selected successfully |
| 7 | Click "Add" button | Inline validation error appears above Email: "Required". Employee is **not** created. |

---

### Test Case C3: Verify that a new Tier can be added successfully from the settings page

**Priority:** High  
**Type:** Smoke & Sanity  

**Precondition:** HR user is logged in and on the **Settings** page

**Steps and Expected Results:**

| Step | Action | Expected Result |
|------|--------|-----------------|
| 1 | Click on "Add Tier" button | "Add Tier" form is opened |
| 2 | Enter "Benefiti" into the Tier Name field | Name is entered without validation error |
| 3 | Enter "Novi Benefiti" into the Description field | Description is entered successfully |
| 4 | Enter "1000" in currency field | 50 tokens are automatically calculated and shown |
| 5 | Click "Add" button | Success message appears: "Tier successfully created!" and "Benefiti" appears in Tier list |

---
