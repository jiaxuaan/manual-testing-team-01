# Manual Testing Results — Member E

## Environment

| Item | Details |
|---|---|
| Tester identifier | member-e |
| Date and time | 5/11/2026 |
| Browser and version | Chrome 157.0.8103.39 |
| Operating system | Windows 11 |

## Login Tests
### Test ID: LOGIN-R01

| Item | Details |
|---|---|
| Test type | Recovery |
| Tester | member-e |
| Website | Swag Labs (saucedemo.com) |
| Status | Pass |

#### Purpose

This test checks that if the user enters the wrong password initially, the login is rejected, and if the password is corrected the login is successful.

#### Preconditions

- User must be logged out initially
- Input fields start empty
- User has tried an invalid login before

#### Test Data

| Field | Value |
|---|---|
| Username | standard_user |
| Password | wrong_password |
| Password | secret_sauce |

#### Steps

1. Enter standard_user and wrong_password.
2. Select Login.
3. Confirm rejection.
4. Replace the password with secret_sauce.
5. Keep the username unchanged.
6. Select Login again.
7. Check whether the inventory appears.

#### Expected Result

The invalid attempt is rejected. After correcting the password, login succeeds.

#### Actual Result

The invalid login attempt is rejected and an error message is displayed. After correcting the password, login succeeds and the inventory page with products is visible.

#### Evidence
Rejection of wrong password:

![login failed with wrong password](../evidence/member-e/login_rejection.png)



Successfully reached inventory page after correction:

![login succeeded after password was corrected](../evidence/member-e/login_success.png)

---

## Equivalence Partitioning
### Test ID: AGE-EP-abc-E

| Item | Details |
|---|---|
| Test type | Recovery |
| Tester | member-e |
| Website | Client Server Form Validation Testing App (testpages.eviltester.com/apps/client-server-form-validation/) |
| Status | Observation only |

#### Purpose

This test checks whether the user can enter abc as an age value, and whether it is accepted or rejected.

#### Preconditions

- All other baseline values are unchanged

#### Test Data

| Field | Value |
|---|---|
| First name | Alex |
| Surname | TestingStudent |
| Age | abc |
| Country | Singapore |
| Notes | Manual testing classroom exercise

#### Steps

1. Restore the form.
2. Enter the valid baseline.
3. Change only age.
4. Write the expected result.
5. Submit.
6. Observe acceptance or rejection.
7. Where displayed, verify the submitted age.
8. Record the actual result and status in a separate test-case block.

#### Actual Result

- The input cannot be entered in the field at all.
- If "submit" is clicked, An error message appears prompting to fill out the age field (it is considered empty)
- Requirement defines the expected behaviour as the age value only accepts numerical values between 18 and 80.

#### Evidence
"abc" can't be entered and if "submit" is clicked anyway an error message appears:

!["abc" is not considered an age](../evidence/member-e/abc_is_not_age.png)


## 2-Point Boundary Tests

## 3-Point Boundary Tests

