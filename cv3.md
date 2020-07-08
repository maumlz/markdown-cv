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
          <h2>Objetivos</h2>
        </div>
      </div>
      <div class="col2">
      </div>
      <div class="col3">
        {% for data in site.data.cv_data %} {{data.goals}} {% endfor %}
      </div>
  </div>
  <div class="row">
      <div class="col1">
        <div class="col4">
          <h2>Conocimiento en</h2>
        </div>
      </div>
      <div class="col2">
      </div>
      <div class="col3">
        {% for data in site.data.cv_data %} {{data.known}} {% endfor %}
      </div>
  </div>

  <div class="row">
    {% for data in site.data.cv_data %}
      <div class="col1">
        <div class="col4">
          <h2>Educación</h2>
        </div>
        <div class="col5">
          {{ data.date }}
        </div>
      </div>
      <div class="col2">
      </div>
      <div class="col3">
        {{data.edu}} {{data.school}}
      </div>
    {% endfor %}
  </div>

  <div class="row">
      <div class="col1">
        <div class="col4">
          <h2>Experiencia</h2>
        </div>
      </div>
      <div class="col2">
      </div>
      <div class="col3">
        {% include experiencia.md %}
      </div>
  </div>

</div>
