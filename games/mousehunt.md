---
layout: page
title: MouseHunt
collection: mousehunt
---

{: .box-note}
This is the longest online game that I still played up to today. Basic of the game is to hunt every 15 minutes

{% for row in site.data.images %}
{% if row["collection"] == page.collection %}![{{row["caption"]}}]({{row["link"] | replace: "image/upload", "image/upload/q_auto:eco"}}){:width="100%" class="col-lg-5"}{% endif %}{% endfor %}