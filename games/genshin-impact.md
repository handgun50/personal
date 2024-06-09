---
layout: page
title: Genshin Impact
collection: genshin
---

{: .box-note}
The game is very nice actually. The grinding is fine, but I just don't have much time to play on laptop. The mobile version uses too many storage on my phone so I didn't install it on my phone. The game also getting bigger and bigger and my laptop is getting laggier especially on Dragonspine.

{% for row in site.data.images %}
{% if row["collection"] == page.collection %}
![{{row["caption"]}}]({{row["link"] | replace: "image/upload", "image/upload/q_auto:eco"}}){:width="100%"}
{% endif %}
{% endfor %}