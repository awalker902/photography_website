---
title: "Contact"
---

<style>
    /* Darkroom Form Styling */
    .contact-form {
        max-width: 500px;
        margin-top: 40px;
    }

    .form-group {
        margin-bottom: 25px;
    }

    label {
        display: block;
        margin-bottom: 8px;
        font-size: 0.9rem;
        color: var(--text-muted);
        letter-spacing: 0.05em;
        text-transform: uppercase;
        font-weight: 700;
    }

    input, textarea {
        width: 100%;
        padding: 12px;
        background-color: var(--bg-panel); /* Dark Grey */
        border: 1px solid var(--border);
        color: var(--text-main);
        font-family: 'Bitter', serif; /* Matching your site font */
        font-size: 1rem;
        box-sizing: border-box;
        transition: border-color 0.2s;
    }

    input:focus, textarea:focus {
        outline: none;
        border-color: var(--text-main); /* Light up on focus */
    }

    button[type="submit"] {
        background-color: transparent;
        color: var(--text-main);
        border: 1px solid var(--text-main);
        padding: 12px 30px;
        font-family: 'Bitter', serif;
        font-weight: 700;
        text-transform: uppercase;
        letter-spacing: 0.1em;
        cursor: pointer;
        transition: all 0.3s;
    }

    button[type="submit"]:hover {
        background-color: var(--text-main);
        color: var(--bg-dark);
    }
</style>

<div class="contact-text">
    <p>For print inquiries or commissions, please use the form below.</p>
</div>

<form name="contact" method="POST" data-netlify="true" netlify-honeypot="bot-field" class="contact-form">
    
<p style="display:none">
    <label>Don’t fill this out if you're human: <input name="bot-field" /></label>
</p>

<div class="form-group">
    <label for="name">Name</label>
    <input type="text" id="name" name="name" required />
</div>

<div class="form-group">
    <label for="email">Email</label>
    <input type="email" id="email" name="email" required />
</div>

<div class="form-group">
    <label for="message">Message</label>
    <textarea id="message" name="message" rows="6" required></textarea>
</div>

<button type="submit">Send Message</button>

</form>