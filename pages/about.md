---
layout: page
title: About
permalink: /about/
weight: 3
---

# **About Me**

Hi I am **{{ site.author.name }}** :wave:,<br>
I recently graduated from college with a bachelors in Network Administration. I have strong interests in networking and virtualization as well as interests in cybersecurity and programming. Recently I've been dipping my toes in different scripting languages for use with services and applications in my home lab. My goal is to gain experience in the field of IT and learn as much as I can along the way.

<div class="row">
{% include about/skills.html title="Skills" source=site.data.skills %}
{% include about/skills.html title='<br>' source=site.data.skills2 %}
{% include about/certifications.html title="Certifications" source=site.data.certifications %}
</div>

<div class="row">
{% include about/timeline.html %}
</div>
