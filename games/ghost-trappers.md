---
layout: page
title: Ghost Trappers Classic
collection: gtc
---

{: .box-note}
This game is similar to MouseHunt, but in this game we can reduce the hunting time until 2 minutes. This game is new version of GT because the old one already closed. But I actually don't like it very much because the website is so laggy and very very unoptimized. For very simple passive game, the laptop fan will go max speed because it's poorly optimized

{% for row in site.data.images %}
{% if row["collection"] == page.collection %}
![{{row["caption"]}}]({{row["link"] | replace: "image/upload", "image/upload/q_auto:eco"}}){:width="100%"}
{% endif %}
{% endfor %}