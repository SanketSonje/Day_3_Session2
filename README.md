# 📝 Accessible Signup Form

A simple and accessible **signup form** built using **semantic HTML**.  
This project demonstrates best practices in **form accessibility**, including labels, fieldsets, ARIA attributes, and keyboard navigability.

## 🔹 Overview
Forms are often the most critical part of any application. However, poorly designed forms create barriers for users with disabilities.  

This signup form was built with accessibility in mind:
- Works with screen readers.
- Fully keyboard navigable.
- Provides proper labels, landmarks, and required attributes.

---

## 🔹 Features
- **Semantic HTML5** structure.  
- **Labels and Inputs** correctly linked (`for` + `id`).  
- **Fieldsets + Legends** to group related form controls.  
- **Required attributes** with `aria-required="true"` for screen readers.  
- **Keyboard accessible** (Tab navigation).  
- **Accessible links** with descriptive text.  

---

## 📂 Deliverables
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

What I Learned

How to build accessible forms with label, fieldset, and legend.
How to use ARIA (aria-required, aria-labelledby) responsibly.
How to test forms with keyboard navigation and screen readers.
How to validate accessibility with Lighthouse.
