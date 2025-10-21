---
layout: page
title: About
permalink: /about/
weight: 3
---

<div class="row mt-4">

  <div class="col-md-4 text-center">

    <div id="container" class="my-2" style="max-width: 250px; margin-left: auto; margin-right: auto;">
      <div id="dummy"></div>
      <div id="element">
        <img src="{{ site.author.image }}" alt="{{ site.author.name | default: site.title }}" class="circle-image wow animated zoomIn" data-wow-delay=".1s">
      </div>
    </div>
        <div class="wow animated slideInUp">
            <p class="text-muted mt-2 mb-3">{{ site.description }}</p>
            {% include social.html %}
        </div>
    </div>

  <div class="col-md-8 mt-4 mt-md-0 markdown-body">

    <h1 class="wow animated fadeIn" data-wow-delay=".1s"><b>About Me</b></h1>

    <div class="wow animated fadeIn" data-wow-delay=".15s">
    <p>Hi I am <b>{{ site.author.name }}</b> :wave:,<br>
    By day, I work as a Network Architect, designing and implementing enterprise network solutions. My professional experience involves working extensively with technologies like Aruba Central, ClearPass, Cisco Catalyst Center, and configuring complex network environments.</p>
    <p>Outside of work, my passion for technology continues in my home lab. I enjoy experimenting with self-hosting and virtualization, primarily using TrueNAS as the core of my setup.</p>
    <p>This site serves as a place to share some of my projects, thoughts on technology, and learnings from both my professional work and personal explorations.</p>
    </div>

  </div>

</div> <div class="row mt-4 wow animated fadeIn" data-wow-delay=".2s">
  {% include about/skills.html title="Programming Skills" source=site.data.programming-skills %}
  {% include about/skills.html title="Other Skills" source=site.data.other-skills %}
</div>
<div class="mt-5 wow animated fadeIn" data-wow-delay=".25s">
  <h2 class="mb-4 text-left">Certifications</h2>
  {% if site.data.certifications %}
    <div class="row justify-content-center">
     {% for cert in site.data.certifications %}
        {% include about/certification-card.html certification=cert cert_col_class='col-md-6' %} {% comment %} Adjust columns: 2 on medium, 3 on large screens {% endcomment %}
     {% endfor %}
    </div>
  {% else %}
    <div class="col-12 text-center text-muted">
      <p>No certifications listed yet.</p>
    </div>
  {% endif %}
</div>
<div class="wow animated fadeIn" data-wow-delay=".25s">
  <h2 class="mb-4 text-left">Timeline</h2>
  {% include about/timeline.html %}
</div>