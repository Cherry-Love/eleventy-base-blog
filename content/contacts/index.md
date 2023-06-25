---
layout: layouts/base.njk
eleventyNavigation:
  key: Contacts
  order: 6
---
# Contacts

<form id="contact-form" name="contact-form" method="POST" netlify>
  <div class="mb-3">
    <label for="contact-email" class="form-label"  >Email address</label>
    <input type="email" class="form-control" id="contact-email" name="contact-email" aria-describedby="emailHelp" placeholder="name@example.com" required>
    <div id="emailHelp" class="form-text">We'll never share your email with anyone else.</div>
  </div>
  <div class="mb-3">
    <label for="contact-name" class="form-label" >Your name</label>
    <input type="text" class="form-control" id="contact-name"  id="contact-name"  required placeholder="Name ..." >
  </div>
	 <div class="mb-3">
    <label for="contact-tel" class="form-label" >Your phone</label>
    <input type="tel" class="form-control" id="contact-tel"  id="contact-tel"  required placeholder="0123456789" >
  </div>
  <div class="mb-3">
  <label for="contact-message" class="form-label" >Your message</label>
  <textarea class="form-control" id="contact-message" rows="3" placeholder="Type your message here ..."  required></textarea>
</div>

  <input type="submit" class="btn btn-primary" id="submit">
</form>
