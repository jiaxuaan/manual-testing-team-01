# Manual Testing Results — Member B

## Environment

| Item | Details |
|---|---|
| Tester identifier | member-a |
| Date and time | |
| Browser and version | |
| Operating system | |

## Login Tests
### Test ID: LOGIN-N01

| Item | Details |
|---|---|
| Test type | Negative |
| Tester | member-b |
| Website | SauseDemo |
| Status | Pass |

#### Purpose

What does this test check?
Checks that an incorrect password rejects login.

#### Preconditions

What must be true before the test starts?
The user is not logged in.

#### Test Data

| Field | Value |
|---|---|
| Username | `standard_user` |
| Password | `wrong_password` |

#### Steps

1. Follow the shared starting procedure.
2. Enter the valid username.
3. Enter the incorrect password.
4. Select Login.
5. Observe the page and feedback.

#### Expected Result

Login is rejected, error feedback appears, and the inventory is not reached.

Keep the username valid to isolate the incorrect-password condition.

If rejection occurs as expected, mark the test Pass.

#### Actual Result

Login is rejected and error popup appears. User is not logged in.

#### Evidence

[View screenshot](/manual-testing/evidence/member-b/login_n01.png)

---

## Equivalence Partitioning

### Test ID: AGE-EP-10-B

| Item | Details |
|---|---|
| Test type | Negative |
| Tester | member-b |
| Website | https://testpages.eviltester.com/apps/client-server-form-validation/submit |
| Status | Pass |

#### Purpose

Checks that an age below 18 is rejected.


#### Preconditions

Any previous queries are cleared

#### Test Data

| Field | Value |
|---|---|
| First Name | `Alex` |
| Last Name | `TestingStudent` |
| Age | `10` |
| Country | `Singapore` |
| Notes | `Manual testing classroom exercise` |

#### Steps

1. Restore the form.
2. Enter the valid baseline.
3. Change only age.
4. Submit.
5. Observe acceptance or rejection.
6. Where displayed, verify the submitted age.

#### Expected Result

The age is rejected and query is not submitted. An error appears.

#### Actual Result

The age is rejected and query is not submitted. An error appears.

#### Evidence

[View screenshot](/manual-testing/evidence/member-b/age-ep-10-b.png)

---


## 2-Point Boundary Tests

## 3-Point Boundary Tests
