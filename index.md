---
width: full
navbar:
  sticky: true
  scroll_up: true
  animation: true
  transparent: true
  transparent_color: light
header:
  layout: 1-1 # Options: left, center, 1-1, 1-2, 1-3 or 2-3
  background_image: Working-Space.jpg
  background_video: Working-Space.mp4
  background_overlay: "linear-gradient(to left top,rgba(218, 91, 197, 0.8) 0%,rgba(151, 27, 191, 0.8) 30%,rgba(2, 8, 212, 0.8) 80%)"
  color: light
  heading_size: medium
  height: full
  parallax: true
  container: small
  content:
    block: header-home
---

[comment]: # (This actually is the most platform independent comment)

{% if site.template == 'base' %}

  {% include slider.html 
  section_size="large"
  section_padding_remove="bottom"
  section_title="" 
  section_header_align="center"
  section_container="xsmall"
  color="light"
  block="slider-home" 
  navigation="outside"
  grid="1-1"
  gutter="collapse"
  %}

  {% include cards.html 
    block="feature-2" 
    section_background="default" 
    section_size="large"
    section_title="We Offer All Kinds of Services" 
    section_header_align="center"
    section_content_align="center"
    media="top"
    grid="1-3"
    gutter="large"
    icon_color="#1B33BF"
  %}

  {% include cards.html 
    block="card-media-12" 
    media="left" 
    section_size="large"
    section_background="default"
    section_header_align="center"
    card_style="default"
  %}

  {% include cards.html 
    block="home-why" 
    section_title="Why use Eon theme?"
    section_header_align="center"
    section_size="large"
    section_background="muted"
    grid="1-3"
    gutter="large"
  %}

  {% include map.html 
    latitude="19.419897" 
    longitude="-99.164967" 
    zoom="12" 
    section_size="medium"
    section_padding_remove="top"
    section_container="small"
    height="large"
  %}
  
{% else %}


{% endif %}