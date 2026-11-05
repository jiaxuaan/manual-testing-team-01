# Manual Testing Results — Member D

## Environment

| Item | Details |
|---|---|
| Tester identifier | member-d |
| Date and time | 5/11/26 10:54am |
| Browser and version | Google Chrome 156.0.8078.80 |
| Operating system | Windows |

## Login Tests
### Test ID: N03 - Missing Password

| Item | Details |
|---|---|
| Test type | Negative | 
| Tester | member-d |
| Website | https://www.saucedemo.com/ |
| Status | Pass |

#### Purpose

Check that SauceDemo rejects a login attempt when the username is left empty, even though the password is valid. The username is the only invalid condition, so any rejection can be traced to it.


#### Preconditions

- The SauceDemo login page (https://www.saucedemo.com/) is open.
- The shared starting procedure has been done: logged out, both fields cleared, and starting from the logged-out state.
- The password to use is the demo one, `secret_sauce`.

#### Test Data

| Field | Value |
|---|---|
| username | secret_sauce |

#### Steps

1. Follow the shared starting procedure.
2. Leave the username empty.
3. Enter the password.
4. Select Login.
5. Observe the feedback

#### Expected Result

The attempt is rejected with validation feedback. The inventory is not reached.

#### Actual Result
The username was empty and I only filled it the password field and the login was not successful.

#### Evidence

Captured.

---


## Equivalence Partitioning

#### Actual Result
Whether the input can be entered: Yes. The age box is a number field with up and down arrows, and it let me leave it empty and select Submit.
Whether it is prevented, cleared, or rejected: Rejected by the browser. Submit was blocked and the page didn’t go through. This was the browser’s built-in check, not the server, so don’t describe it as a server response.
What feedback appears: A small browser pop-up under the age field saying “Please fill out this field.” The cursor also lands in the age box.
Whether the requirement clearly defines the expected behaviour: Not really. The requirement table only says age is between 18 and 80, and it doesn’t say what a blank age should do. So I’d write it as an observation (or a requirement question) instead of marking Pass/Fail, and say you assumed a blank age shouldn’t be accepted.
### Test ID: AGE-EP-Blank-D


## 2-Point Boundary Tests

## 3-Point Boundary Tests