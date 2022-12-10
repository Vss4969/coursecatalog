---
layout: page
---


<div class="header">
        <img class="indexpic" src="assets/indexpic.png" alt="indexpic">
</div>


<div>
<hr>
<ul>
{% for course in site.courses %}
    <li><a href="{{course.url | relative_url}}">{{course.title}}</a></li>
{% endfor %}
</ul>
</div>


<hr>
<div class="footer">
    <h1>Footer</h1>
</div>