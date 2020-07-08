---
layout: gridview
title: Mauricio Meléndez
---
<div class="page">
  <div class="row">
      <div class="col1">

      </div>
      <div class="col2">

      </div>
      <div class="col3">
        <h1>{% for data in site.data.cv_data %} {{data.name}} {% endfor %}</h1>
      </div>
  </div>
  <div class="row">
      <div class="col1">
        <div class="col4">
          Objetivos
        </div>
      </div>
      <div class="col2">

      </div>
      <div class="col3">
        {% site.data.c_data.goals %}
      </div>
  </div>
</div>
