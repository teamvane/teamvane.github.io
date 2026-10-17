---
title: Contact
permalink: /contact/
description: How to reach Teamvane for support, sales questions and security reports.
---

# Contact

We're a small team and we read every message. Write in English, French or Spanish.

<div class="contact-cards">
  <div class="contact-card">
    <h2>Support and questions</h2>
    <p>Help with the apps, bug reports, licensing and anything else.</p>
    <p class="contact-address"><a href="mailto:support@teamvane.com">support@teamvane.com</a> <button type="button" class="copy" data-copy="support@teamvane.com">Copy</button></p>
    <p class="contact-note">We reply within one business day (Monday to Friday, except French public holidays).</p>
  </div>
  <div class="contact-card">
    <h2>Security</h2>
    <p>Report a vulnerability in one of our apps.</p>
    <p class="contact-address"><a href="mailto:security@teamvane.com">security@teamvane.com</a> <button type="button" class="copy" data-copy="security@teamvane.com">Copy</button></p>
    <p class="contact-note">See our <a href="/security/">security policy</a> for what to include and how we respond.</p>
  </div>
</div>

<script>
  // "Copy" buttons: put the address on the clipboard, for visitors whose
  // computer doesn't open email links.
  document.querySelectorAll('button.copy').forEach(function (button) {
    button.addEventListener('click', function () {
      navigator.clipboard.writeText(button.dataset.copy).then(function () {
        button.textContent = 'Copied';
        setTimeout(function () { button.textContent = 'Copy'; }, 2000);
      });
    });
  });
</script>
