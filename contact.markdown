---
layout: page
title: Contact Us
permalink: contact
---

<h3>Send us a Message</h3>
<form name="sentMessage" id="contactForm" novalidate action="https://formspree.io/{{ site.email }}" method="POST">
  <div class="control-group form-group">
      <div class="controls">
          <label>Full Name:</label>
          <input type="text" class="form-control" id="name" required data-validation-required-message="Please enter your name.">
          <p class="help-block"></p>
      </div>
  </div>
  <div class="control-group form-group">
      <div class="controls">
          <label>Phone Number:</label>
          <input type="tel" class="form-control" id="phone" required data-validation-required-message="Please enter your phone number.">
      </div>
  </div>
  <div class="control-group form-group">
      <div class="controls">
          <label>Email Address:</label>
          <input type="email" class="form-control" id="email" required data-validation-required-message="Please enter your email address.">
      </div>
  </div>
  <div class="control-group form-group">
      <div class="controls">
          <label>Message:</label>
          <textarea rows="10" cols="100" class="form-control" id="message" required data-validation-required-message="Please enter your message" maxlength="999" style="resize:none"></textarea>
      </div>
  </div>
  <div id="success"></div>
  <input type="hidden" name="_next" value="contact" />
  <!-- For success/fail messages -->
  <button type="submit" class="btn btn-primary">Send Message</button>
</form>
