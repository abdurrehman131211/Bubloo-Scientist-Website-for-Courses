# Bubloo Scientist Academy — AI That Actually Works

## Registration form setup
The website supports Google Forms and Microsoft Forms without requiring a custom backend.

### Easiest setup
1. Open the deployed site.
2. Scroll to Registration.
3. Click **Configure form**.
4. Select Google Forms or Microsoft Forms.
5. Paste your form's share link.
6. Click **Save & display form**.

The site embeds the form. The learner's answers are submitted directly to your chosen provider, so your Google Forms/Microsoft Forms response system remains the source of truth.

### Important static-site limitation
The browser stores the configured form URL in localStorage. That means configuring the form on one computer does not automatically configure every visitor's browser.

For a permanent deployment, edit the `FORM_CONFIG` object at the top of `app.js`:

```js
const FORM_CONFIG={
  provider:'google',
  url:'PASTE_YOUR_FORM_LINK_HERE'
};
```

Use `microsoft` for Microsoft Forms.

The website also keeps the setup UI so you can change the form later without changing the page structure.

## Form fields recommended
- Full name
- Email address
- WhatsApp/contact number (optional)
- Student/professional status
- Why do you want to learn AI?
- What AI tools have you used?
- What do you struggle with most?
- How did you hear about Bubloo Scientist?
- Consent to receive course information

Do not collect unnecessary sensitive information.

## Payment
The current registration flow intentionally does not pretend to have a payment processor. You can collect registrations first and manually follow up, or later connect the CTA to a real checkout/payment workflow.
