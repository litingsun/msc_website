---
layout: page-wide
title: Students
permalink: /people/students.html
---

{% if site.data.post_docs.size >= 1 %}
  <div class="people">
    <h2 class="sub-heading">Post-Docs</h2>
    <div class="container-fluid">
      <div class="person-images">
        {% for post_doc in site.data.post_docs %}
          <div class="person-member">
            <div class="person-image">
              <img src="../assets/images/people/{{ post_doc.image }}.jpg" alt="">
              <img src="../assets/images/people/{{ post_doc.image }}1.jpg" alt="">
            </div>
            <div class="person-description">
              <div class="person-name">{{ post_doc.name }}</div>
                <p>{{ post_doc.title }}</p>
              {% if post_doc.email %}
                <p><a href="mailto:{{ post_doc.email }}" target="_new">Email</a> |
              {% else %}
                <p> Email |
              {% endif %}
              {% if post_doc.homepage %}
                <a href="{{ post_doc.homepage }}" target="_new">Homepage</a></p>
              {% else %}
                Homepage </p>
              {% endif %}
            </div>
          </div>
        {% endfor %}
      </div>
    </div>
  </div>
{% endif %}

<div class="people">
  <h2 class="sub-heading">PhD Students</h2>
  <div class="container-fluid">
    <div class="person-images">
      {% for student in site.data.students %}
      <div class="person-member">
        <div class="person-image">
          <img src="../assets/images/people/{{ student.image }}.jpg" alt="">
          <img src="../assets/images/people/{{ student.image }}1.jpg" alt="">
        </div>
        <div class="person-description">
          <div class="person-name">{{ student.name }}</div>
          <p>{{ student.title }}</p>
          {% if student.email %}
          <p><a href="mailto:{{ student.email }}" target="_new">Email</a> |
          {% else %}
          <p> Email |
          {% endif %}
          {% if student.homepage %}
          <a href="{{ student.homepage }}" target="_new">Homepage</a></p>
          {% else %}
          Homepage </p>
          {% endif %}
        </div>
      </div>
      {% endfor %}

    </div>
  </div>
</div>

{% if site.data.masters.size >= 1 %}
<div class="people">
    <h2 class="sub-heading">Master Students</h2>
        <div class="container-fluid">
        <div class="person-images">
        {% for master in site.data.masters %}
            <div class="person-member">
            <div class="person-image">
            <img src="../assets/images/people/{{ master.image }}.jpg" alt="">
            <img src="../assets/images/people/{{ master.image }}1.jpg" alt="">
            </div>
            <div class="person-description">
            <div class="person-name">{{ master.name }}</div>
            <p>{{ master.title }}</p>
            {% if master.email %}
                <p><a href="mailto:{{ master.email }}" target="_new">Email</a> |
            {% else %}
                <p> Email |
            {% endif %}
            {% if master.homepage %}
                <a href="{{ master.homepage }}" target="_new">Homepage</a></p>
            {% else %}
                Homepage </p>
            {% endif %}
            </div>
            </div>
        {% endfor %}
        </div>
    </div>
</div>
{% endif %}