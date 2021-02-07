---
layout: page
permalink: /
title: about
nav: about
---

<div class="text-center mt-5">
  <img class="profile-img" src="{{ site.profile_imgs[3] | prepend: '/assets/img/' | prepend: site.baseurl | prepend: site.url }}">
</div>

<div class="col mt-4">
  <h1 class="title text-center font-weight-bold">Sanjana Mendu</h1>
  <div class="row mt-3 mb-3">
    <div class="col-sm-6">
  </div>
</div>

<!-- Introduction -->

<div class="col text-center p-0">
  I am a first-year Ph.D. student studying 
  <a href="https://ist.psu.edu/prospective/graduate/phd-informatics" target="_blank">Informatics</a> in the 
  <a href="https://ist.psu.edu/" target="_blank">College of Information Sciences and Technology</a> at the 
  <a href="https://www.psu.edu/" target="_blank">Pennsylvania State University</a>. 
  My advisor is <a href="https://saeedabdullah.com" target="_blank">Dr. Saeed Abdullah</a> and I work on designing, developing, and deploying novel sensing and intervention systems focusing on health and wellbeing.
  
  <br/><br/>

  Before I joined Penn State, I graduated with 
  a BS in <a href="https://engineering.virginia.edu/departments/computer-science" target="_blank">Computer Science</a> 
  and an MS in <a href="https://engineering.virginia.edu/departments/engineering-systems-and-environment/academics/systems-engineering" target="_blank">Systems Engineering</a> from the <a href="https://www.virginia.edu" target="_blank">University of Virginia</a>. 
  For my <a href="https://libraetd.lib.virginia.edu/public_view/xg94hq166" target="_blank">Master's thesis</a>, I proposed a novel framework for constructing rich feature spaces from digital text communications.
</div>

<!-- News -->
<div class="news mt-5 p-0">
  <h2 class="title mb-2 p-0">news</h2>
  <h4 class="p-0" style="color:gray;">[ <i>coming soon</i> ]</h4>
  <!-- {% assign news = site.news | reverse %}
  {% for item in news limit: site.news_limit %}
    <div class="row p-0">
      <div class="col-sm-2 p-0">=
        <span class="badge badge-primary badge-pill text-uppercase align-middle date ml-3">
          {{ item.date | date: "%b %Y" }}
        </span>
      </div>
      <div class="col-sm-10 mt-2 mt-sm-0 ml-3 ml-md-0 p-0 font-weight-light text">
        <p>{{ item.content | remove: '<p>' | remove: '</p>' | emojify }}</p>
      </div>
    </div>
  {% endfor %} -->
</div>