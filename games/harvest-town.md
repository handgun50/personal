---
layout: page
title: Harvest Town
collection: harvesttown
---

{: .box-note}
I like harvest moon, so this game is similar with it. Maybe Stardew Valley is better (I haven't tried it), but since this game is free and not very heavy, it is quite good.

{% for row in site.data.images %}
{% if row["collection"] == page.collection %}
![{{row["caption"]}}]({{row["link"] | replace: "image/upload", "image/upload/q_auto:eco"}}){:width="100%"}
{% endif %}
{% endfor %}


