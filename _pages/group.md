---
title: "Denolle Quake Lab - Group"
layout: gridlay
excerpt: "Denolle Quake Lab: Group members"
sitemap: false
permalink: /group/
---

# Group Members
---
 **We are  looking for new PhD students, Postdocs, and Master students to join the team** [(see openings)]({{ site.url }}{{ site.baseurl }}/openings) **!**
 For new applicants and incoming group members, please see our [group guidelines](https://github.com/Denolle-Lab/working_as_a_group/blob/main/onboarding.md).

Our group defined a [working contract](https://github.com/Denolle-Lab/working_as_a_group/blob/main/Work_contract.md).

Jump to [staff](#staff), [postdoc](#postdoc), [graduate students](#graduate),[undergraduate students](#undergraduate),  [alumni](#alumni).

<!-- ## Staff ------------------------------->
{% assign number_printed = 0 %}
{% for member in site.data.team_members %}

{% assign even_odd = number_printed | modulo: 2 %}

{% if even_odd == 0 %}
<div class="row">
{% endif %}

<div class="col-sm-6 clearfix">
  <img src="{{ site.url }}{{ site.baseurl }}/images/teampic/{{ member.photo }}" class="img-responsive" width="25%" style="float: left" />
  <h4>{{ member.name }}</h4>
  <br> {{ member.info }}  <br><b>email </b>: <{{ member.email }}>  <br><b> PhD </b>: {{ member.education1 }}  
 
  <ul style="overflow: hidden">

 {% if member.number_educ == 1 %}
  <li> {{ member.education1 }} </li>
  {% endif %}

  {% if member.number_educ == 2 %}
  <li> {{ member.education1 }} </li>
  <li> {{ member.education2 }} </li>
  {% endif %}

  {% if member.number_educ == 3 %}
  <li> {{ member.education1 }} </li>
  <li> {{ member.education2 }} </li>
  <li> {{ member.education3 }} </li>
  {% endif %}

  {% if member.number_educ == 4 %}
  <li> {{ member.education1 }} </li>
  <li> {{ member.education2 }} </li>
  <li> {{ member.education3 }} </li>
  <li> {{ member.education4 }} </li>
  {% endif %} 

  {% if member.number_educ == 5 %}
  <li> {{ member.education1 }} </li>
  <li> {{ member.education2 }} </li>
  <li> {{ member.education3 }} </li>
  <li> {{ member.education4 }} </li>
  <li> {{ member.education5 }} </li>
  {% endif %} 
  </ul>
</div>

{% assign number_printed = number_printed | plus: 1 %}

{% if even_odd == 1 %}
</div>
{% endif %}

{% endfor %}

{% assign even_odd = number_printed | modulo: 2 %}
{% if even_odd == 1 %}
</div>
{% endif %}

<!-- ------------- POSTDOC ----------- -->
## Postdocs

{% assign number_printed = 0 %}
{% for member in site.data.postdocs %}

{% assign even_odd = number_printed | modulo: 2 %}

{% if even_odd == 0 %}
<div class="row">
{% endif %}

<div class="col-sm-6 clearfix">
<img src="{{ site.url }}{{ site.baseurl }}/images/teampic/{{ member.photo }}" class="img-responsive" width="25%" style="float: left" /> 
  <h4>{{ member.name }}</h4>
  {{ member.info }}  <br><b>email </b>: <{{ member.email }}>  <br><b> PhD </b>: {{ member.education }} <br> <b> Postdoc Research </b>: {{ member.info2 }} <br> <b> Webpage </b>: {{ member.info3 }} <br> <b>Github </b>: {{ member.info4 }}  
  <ul style="overflow: hidden">

  <!-- {% if member.number_educ == 1 %}
  <li> {{ member.education1 }} </li>
  {% endif %}

  {% if member.number_educ == 2 %}
  <li> {{ member.education1 }} </li>
  <li> {{ member.education2 }} </li>
  {% endif %}


  {% if member.number_info == 2 %}
  <li> {{ member.info }} </li>
  <li> {{ member.info2 }} </li>
  {% endif %}


  {% if member.number_info == 3 %}
  <li> {{ member.info }} </li>
  <li> {{ member.info2 }} </li>
  <li> {{ member.info3 }} </li>
  {% endif %}


  {% if member.number_educ == 3 %}
  <li> {{ member.education1 }} </li>
  <li> {{ member.education2 }} </li>
  <li> {{ member.education3 }} </li>
  {% endif %}  -->


  <!-- {% if member.number_info== 4 %}
  <li> {{ member.info }} </li>
  <li> {{ member.info2 }} </li>
  <li> {{ member.info3 }} </li>
  <li> {{ member.info4 }} </li>
  {% endif %} -->

<!-- 
  {% if member.number_educ == 4 %}
  <li> {{ member.education1 }} </li>
  <li> {{ member.education2 }} </li>
  <li> {{ member.education3 }} </li>
  <li> {{ member.education4 }} </li>
  {% endif %} -->

  </ul>
</div>

{% assign number_printed = number_printed | plus: 1 %}

{% if even_odd == 1 %}
</div>
{% endif %}

{% endfor %}

{% assign even_odd = number_printed | modulo: 2 %}
{% if even_odd == 1 %}
</div>
{% endif %}


 <!--------------- GRAD   STUDENTS    -------------- -->
## Graduate Students
{% assign number_printed = 0 %}
{% for member in site.data.students %}

{% assign even_odd = number_printed | modulo: 2 %}

{% if even_odd == 0 %}
<div class="row">
{% endif %}

<div class="col-sm-6 clearfix">
<img src="{{ site.url }}{{ site.baseurl }}/images/teampic/{{ member.photo }}" class="img-responsive" width="25%" style="float: left" /> 
  <h4>{{ member.name }}</h4>
  {{ member.info }}  <br><b>email</b>: <{{ member.email }}>  <br><b> PhD and Institution </b>: {{ member.info }} <br> <b> PhD Research </b>: {{ member.info2 }} <br> <b> Webpage </b>: {{ member.info3 }} <br> <b>Github </b>: {{ member.info4 }}  
  <ul style="overflow: hidden">

  <!-- {% if member.number_educ == 1 %}
  <li> {{ member.education1 }} </li>
  {% endif %}

  {% if member.number_educ == 2 %}
  <li> {{ member.education1 }} </li>
  <li> {{ member.education2 }} </li>
  {% endif %}


  {% if member.number_info == 2 %}
  <li> {{ member.info }} </li>
  <li> {{ member.info2 }} </li>
  {% endif %}

  {% if member.number_educ == 3 %}
  <li> {{ member.education1 }} </li>
  <li> {{ member.education2 }} </li>
  <li> {{ member.education3 }} </li>
  {% endif %} -->


  </ul>
</div>

{% assign number_printed = number_printed | plus: 1 %}

{% if even_odd == 1 %}
</div>
{% endif %}

{% endfor %}

{% assign even_odd = number_printed | modulo: 2 %}
{% if even_odd == 1 %}
</div>
{% endif %}

<!-- -------------- UNDERGRADS  ------------------->

## Undergraduate researchers

{% assign number_printed = 0 %}
{% for member in site.data.undergrads %}

{% assign even_odd = number_printed | modulo: 2 %}

{% if even_odd == 0 %}
<div class="row">
{% endif %}

<div class="col-sm-6 clearfix">
<img src="{{ site.url }}{{ site.baseurl }}/images/teampic/{{ member.photo }}" class="img-responsive" width="25%" style="float: left" /> 
  <h4>{{ member.name }}</h4>
  {{ member.info }}  <br><b>email </b>: <{{ member.email }}>  <br><b> Degree Institution </b>: {{ member.info }} <br> <b> Research </b>: {{ member.info2 }}  <br> <b>Github </b>: {{ member.info4 }}  
  <ul style="overflow: hidden">
<!-- 
  {% if member.number_educ == 1 %}
  <li> {{ member.education1 }} </li>
  {% endif %}

  <!-- {% if member.number_educ == 2 %}
  <li> {{ member.education1 }} </li>
  <li> {{ member.education2 }} </li>
  {% endif %}


  {% if member.number_info == 2 %}
  <li> {{ member.info }} </li>
  <li> {{ member.info2 }} </li>
  {% endif %}


  {% if member.number_info == 3 %}
  <li> {{ member.info }} </li>
  <li> {{ member.info2 }} </li>
  <li> {{ member.info3 }} </li>
  {% endif %}


  {% if member.number_educ == 3 %}
  <li> {{ member.education1 }} </li>
  <li> {{ member.education2 }} </li>
  <li> {{ member.education3 }} </li>
  {% endif %} -->
 

  <!-- {% if member.number_info== 4 %}
  <li> {{ member.info }} </li>
  <li> {{ member.info2 }} </li>
  <li> {{ member.info3 }} </li>
  <li> {{ member.info4 }} </li>
  {% endif %} -->

<!-- 
  {% if member.number_educ == 4 %}
  <li> {{ member.education1 }} </li>
  <li> {{ member.education2 }} </li>
  <li> {{ member.education3 }} </li>
  <li> {{ member.education4 }} </li>
  {% endif %} -->

  </ul>
</div>

{% assign number_printed = number_printed | plus: 1 %}

{% if even_odd == 1 %}
</div>
{% endif %}

{% endfor %}

{% assign even_odd = number_printed | modulo: 2 %}
{% if even_odd == 1 %}
</div>
{% endif %}



<!-- -------------- AFFILIATED GRADUATE STUDENTS  ------------------->

## Affiliated Graduate students

{% assign number_printed = 0 %}
{% for member in site.data.othergrads %}

{% assign even_odd = number_printed | modulo: 2 %}

{% if even_odd == 0 %}
<div class="row">
{% endif %}

<div class="col-sm-6 clearfix">
<img src="{{ site.url }}{{ site.baseurl }}/images/teampic/{{ member.photo }}" class="img-responsive" width="25%" style="float: left" /> 
  <h4>{{ member.name }}</h4>
  {{ member.info }}  <br><b>email </b>: <{{ member.email }}>  <br><b> Degree Institution </b>: {{ member.info }} <br> <b> Research </b>: {{ member.info2 }}  <br> <b>Github </b>: {{ member.info4 }}  
  <ul style="overflow: hidden">
<!-- 
  {% if member.number_educ == 1 %}
  <li> {{ member.education1 }} </li>
  {% endif %}

  <!-- {% if member.number_educ == 2 %}
  <li> {{ member.education1 }} </li>
  <li> {{ member.education2 }} </li>
  {% endif %}


  {% if member.number_info == 2 %}
  <li> {{ member.info }} </li>
  <li> {{ member.info2 }} </li>
  {% endif %}


  {% if member.number_info == 3 %}
  <li> {{ member.info }} </li>
  <li> {{ member.info2 }} </li>
  <li> {{ member.info3 }} </li>
  {% endif %}


  {% if member.number_educ == 3 %}
  <li> {{ member.education1 }} </li>
  <li> {{ member.education2 }} </li>
  <li> {{ member.education3 }} </li>
  {% endif %} -->
 

  <!-- {% if member.number_info== 4 %}
  <li> {{ member.info }} </li>
  <li> {{ member.info2 }} </li>
  <li> {{ member.info3 }} </li>
  <li> {{ member.info4 }} </li>
  {% endif %} -->

<!-- 
  {% if member.number_educ == 4 %}
  <li> {{ member.education1 }} </li>
  <li> {{ member.education2 }} </li>
  <li> {{ member.education3 }} </li>
  <li> {{ member.education4 }} </li>
  {% endif %} -->

  </ul>
</div>

{% assign number_printed = number_printed | plus: 1 %}

{% if even_odd == 1 %}
</div>
{% endif %}

{% endfor %}

{% assign even_odd = number_printed | modulo: 2 %}
{% if even_odd == 1 %}
</div>
{% endif %}


<!-- ------------------   ALUMN  ------------------>
## Alumni

{% assign number_printed = 0 %}
{% for member in site.data.alumni_members %}

{% assign even_odd = number_printed | modulo: 2 %}

{% if even_odd == 0 %}
<div class="row">
{% endif %}

<div class="col-sm-6 clearfix">
  <img src="{{ site.url }}{{ site.baseurl }}/images/teampic/{{ member.photo }}" class="img-responsive" width="25%" style="float: left" />
  <h4>{{ member.name }}</h4>
  <b>Date </b>: {{ member.date }} <br> <b>Role </b>: {{ member.info }}  <br> <b>Research </b>: {{ member.info2 }}   <br> <b> Now at </b> : {{ member.info3 }} 
  <ul style="overflow: hidden">

  </ul>
</div>

{% assign number_printed = number_printed | plus: 1 %}

{% if even_odd == 1 %}
</div>
{% endif %}

{% endfor %}

{% assign even_odd = number_printed | modulo: 2 %}
{% if even_odd == 1 %}
</div>
{% endif %}



<!-- ## Administrative Support -->
<!-- <a href="mailto:Rijsewijk@Physics.LeidenUniv.nl">Ellie van Rijsewijk</a> is helping us (and other groups) with administration. -->
