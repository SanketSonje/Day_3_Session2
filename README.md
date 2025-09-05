# Accessible Signup Form

A simple and accessible signup form built using semantic HTML.  
This project demonstrates best practices in form accessibility, including labels, fieldsets, ARIA attributes, and keyboard navigability.

# Overview
the Forms are often the most critical part of any application. However, poorly designed forms create barriers for users with disabilities.  

# Accessibility Testing with Lighthouse

To ensure the form meets accessibility standards, I tested it using **Lighthouse** in Chrome DevTools.  

# Steps to Run the Audit
1. Open `signup.html` in **Google Chrome**.  
2. Right-click → **Inspect** → Go to **Lighthouse** tab.  
3. Select **Accessibility** category.  
4. Click **Generate Report**.  
5. Export the report as `lighthouse-report.html` and commit it to the repo.  

# Expected Results
- **Accessibility Score:** 90–100 (Green rating).  
- **Checks Passed:**  
  - All form controls have associated labels.  
  - Required fields are announced to screen readers.  
  - Links and buttons have sufficient contrast and descriptive text.  
  - Page is fully keyboard-navigable.  

## Deliverables
### 1. `signup.html`
Main form file that includes:

```html
<form aria-labelledby="signup-title">
  <h2 id="signup-title">Create an Account</h2>

  <fieldset>
    <legend>Personal Information</legend>
    <label for="first-name">First Name</label>
    <input type="text" id="first-name" name="first-name" required aria-required="true" />
    
    <label for="last-name">Last Name</label>
    <input type="text" id="last-name" name="last-name" required aria-required="true" />
  </fieldset>

  <fieldset>
    <legend>Account Information</legend>
    <label for="email">Email Address</label>
    <input type="email" id="email" name="email" required aria-required="true" />

    <label for="password">Password</label>
    <input type="password" id="password" name="password" required aria-required="true" />

    <label for="confirm-password">Confirm New Password</label>
    <input type="password" id="confirm-password" name="confirm-password" required aria-required="true" />
  </fieldset>

  <button type="submit">Sign Up</button>

  <div class="login-link">
    <p>Already have an account? <a href="login.html">Log in here</a></p>
  </div>
</form>
```
What I Learned

- How to build accessible forms with label, fieldset, and legend.
- How to use ARIA (aria-required, aria-labelledby) responsibly.
- How to test forms with keyboard navigation and screen readers.
- How to validate accessibility with Lighthouse.
