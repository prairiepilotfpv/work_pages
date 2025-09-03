---
# Feel free to add content and custom Front Matter to this file.
# To modify the layout, see https://jekyllrb.com/docs/themes/#overriding-theme-defaults

layout: page
title: Home
---

Welcome to your new site!

{% if site.show_blog_on_home %}
  {% include latest_posts.liquid %}
{% endif %}
