---
layout: about
title: about
permalink: /
# subtitle: <a href='#'>Affiliations</a>. Address. Contacts. Motto. Etc.

profile:
  align: right
  image: prof_pic.jpg
  image_circular: false # crops the image to make it circular
  more_info: >
    <p>Universität Tübingen</p>
    <p>Deutsches Seminar</p>
    <p>Wilhelmstraße 50, 72074 Tübingen, Germany</p>
    <p>Room 444</p>

selected_papers: false # includes a list of papers marked as "selected={true}"
social: false # includes social icons at the bottom of the page

announcements:
  enabled: true # includes a list of news items
  scrollable: true # adds a vertical scroll bar if there are more than 3 news items
  limit: 5 # leave blank to include all the news in the `_news` folder

latest_posts:
  enabled: false
  scrollable: true # adds a vertical scroll bar if there are more than 3 new posts items
  limit: 3 # leave blank to include all the blog posts
---
<div style="display: flex; flex-direction: column; min-height: 100vh;">
  
  <div>
    <!-- Your main content goes here -->
  I am a researcher in (formal) semantics and pragmatics in the [German Seminar](https://uni-tuebingen.de/fakultaeten/philosophische-fakultaet/fachbereiche/neuphilologie/deutsches-seminar/abteilungen/linguistik/) at the University of Tübingen, Germany.

  For most of my academic life, my research has centered around how temporal information is encoded in natural language. In my dissertation, I investigate the nominal categories of tense and aspect and develop a formal logic that models temporality across domains in a unified way. The thesis will be available on the [publications page](https://maximilianaberthold.github.io/publications/) once it has been published by the university library.

    {% if page.announcements.enabled %}
      {% for item in site.news limit:5 %}
        <div class="announcement">
          <p>{{ item.date | date: "%B %d, %Y" }}</p>
          <p>{{ item.title }}</p>
        </div>
      {% endfor %}
    {% endif %}
  </div>

  <!-- Contact section stays at the bottom -->
  <div style="margin-top: auto;">
    <hr class="fixed-gray-line">

  <p style="font-size: 23px; margin-top: 5px;">
    Contact
  </p>

  maximilian[dot]berthold[at]uni-tuebingen[dot]de
  </div>

</div>
