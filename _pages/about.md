---
title: "About"
layout: gridlay
sitemap: false
permalink: /about/
---


## About

{% for member in site.data.pi %}

<div class="jumbotron">
<div class="row">
<div class="col-sm-4">
  <img src="{{ site.url }}{{ site.baseurl }}/images/{{ member.photo }}" width="100%" style="max-width:250px"/>
</div>
<div class="col-sm-8 col-xs-12">
  <h3>{{ member.name }}</h3>
  <h4><i>{{ member.info }}</i></h4>
  {% if member.email %}<a href="mailto:{{ member.email }}" target="_blank"><i class="fa fa-envelope-square fa-3x"></i></a> {% endif %}
  <!-- {% if member.scholar %} <a href="{{ member.scholar }}" target="_blank"><i class="ai ai-google-scholar-square ai-3x"></i></a> {% endif %} -->
  {% if member.github %} <a href="{{ member.github }}" target="_blank"><i class="fa fa-github-square fa-3x"></i></a> {% endif %}
  {% if member.home %}<a href="{{ member.home }}" target="_blank"><i class="fa fa-home fa-3x"></i></a> {% endif %}
  {% if member.twitter %}<a href="{{ member.twitter }}" target="_blank"><i class="fa fa-twitter-square fa-3x"></i></a> {% endif %}
  <!-- {% if member.researchgate %} <a href="{{ member.researchgate }}" target="_blank"><i class="ai ai-researchgate-square ai-3x"></i></a> {% endif %}
  {% if member.cv %} <a href="{{ site.url }}{{ site.baseurl }}/{{ member.cv }}" target="_blank"><i class="ai ai-cv-square ai-3x"></i></a> {% endif %} -->

  <ul style="overflow: hidden">
    {% for education in member.education %}
      <li>{{ education | replace: "-","&#8211;" }}</li>
    {% endfor %}
  </ul>

</div>
</div>
</div>
{% endfor %}


<div class="jumbotron">
  <h3>Experiences</h3>
  <ul>
     <li> <u>Apr. 2024 - Aug. 2024</u> <br>
            Research Internship, Okinawa Institute of Science and Technology, Japan <br>
            Research Unit: <a href="https://groups.oist.jp/qsu" target="_blank">Quantum System Unit </a> </li>
  </ul>
</div>



<div class="jumbotron">
  <h3>Fellowship</h3>
  <!-- <ul>
    <li> <u>Apr. 2025 - </u> <br> FoPM??? </li>
  </ul> -->
</div>






