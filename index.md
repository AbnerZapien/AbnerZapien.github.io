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
  background_image: stock-original-2.jpg
  background_video: Working-Cleaning.mp4
  background_overlay: "linear-gradient(90deg, rgba(22,20,18,0.8) 0%, rgba(90,71,58,0.8) 35%, rgba(199,189,177,0.8) 100%)"
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

  {% include block.html 
    block="content-aboutUs"
    block_title="false"
    section_size="large"
    section_title="About Us"
    section_background="#c7bdb1"
    section_container="xsmall"
    section_header_align="center"
  %}

  {% include slider.html 
    section_title="Meet Our Partners"
    section_header_align="center"
    block="slider-logo" 
    section_size="large"
    section_content_align="center"
    section_background="#ddd9d6"
    display_title="false"
    autoplay="true"
    sets="false"
    grid="1-4"
    gutter="large"
    navigation="outside"
    dotnav="false"
  %}

  {% include cards.html 
  section_title="
  General Services"
  section_header_align="center"
  block="card-media-general" 
  media="top" 
  section_size="large"
  section_container="expand"
  section_background="#c7bdb1"
  card_style="default"
  section_content_align="center"
  %}

  {% include cards.html 
    block="general-service" 
    section_background="#ddd9d6"
    section_size="large"
    section_title="More services!" 
    section_header_align="center"
    section_content_align="center"
    media="top"
    grid="1-3"
    gutter="large"
    icon_color="#1B33BF"
  %}

  {% include slider.html 
    section_title="Our Work"
    section_header_align="center"
    block="slider-works" 
    section_size="large"
    section_content_align="center"
    section_background="#c7bdb1"
    display_title="false"
    autoplay="true"
    sets="false"
    grid="1-4"
    gutter="large"
    navigation="outside"
    dotnav="false"
  %}

  {% include cards.html 
    block="review1" 
    section_background="#ddd9d6"
    section_size="large"
    section_title="What People Say About Us" 
    section_header_align="center"
    section_content_align="center"
    media="top"
    grid="1-1"
    gutter="large"
    icon_color="#1B33BF"
  %}

  {% include map.html 
    latitude="19.419897" 
    longitude="-99.164967" 
    zoom="12" 
    section_size="medium"
    section_container="small"
    height="large"
  %}
  
{% else %}


{% endif %}