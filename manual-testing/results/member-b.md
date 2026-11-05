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

## 2-Point Boundary Tests

## 3-Point Boundary Tests
