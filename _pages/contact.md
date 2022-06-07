---
layout: home
permalink: /contact
 
---

<form>
  <fieldset>
    <legend>Enquiry:</legend>
    Your Name: <input type="text" size="30"><br>
    Email: <input type="email" size="30"><br>
    Enquiry: <textarea rows="10" cols="10"></textarea>
  </fieldset>
  <a href="#" class="btn btn--success" onclick="this.closest('form').submit();return false;">Submit</a>
</form>

{% include feature_row %}
