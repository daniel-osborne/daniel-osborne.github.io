---
layout: page
title: About
permalink: /about/
weight: 3
---

{% capture content %}
# **About Me**

Hi I am {{ site.author.name }} :wave:,<br>
By day, I work as a Network Architect, designing and implementing enterprise network solutions. My professional experience involves working extensively with technologies like Aruba Central, ClearPass, Cisco 

Catalyst Center, and configuring complex network environments.
Outside of work, my passion for technology continues in my home lab. I enjoy experimenting with self-hosting and virtualization, primarily using TrueNAS as the core of my setup.

This site serves as a place to share some of my projects, thoughts on technology, and learnings from both my professional work and personal explorations.
{% endcapture %}

{% include about/profile-banner.html source=content %}

<div class="row mt-4 wow animated fadeIn" data-wow-delay=".2s">
  {% include about/skills.html title="Programming Skills" source=site.data.programming-skills %}
  {% include about/skills.html title="Other Skills" source=site.data.other-skills %}
</div>
<div class="wow animated fadeIn" data-wow-delay=".25s">
  {% include about/certifications.html %}
</div>
<div class="wow animated fadeIn" data-wow-delay=".25s">
  {% include about/timeline.html %}
</div>