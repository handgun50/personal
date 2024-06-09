---
layout: page
title: Homescapes
collection: homescapes
---

{: .box-note}
The game might be very boring for someone, but it's quite fun though. Especially when I get some timed unlimited boosters and timed unlimited health, it makes me forgot the time to repeat and repeat again until finally win.

{% for row in site.data.images %}
{% if row["collection"] == page.collection %}
![{{row["caption"]}}]({{row["link"] | replace: "image/upload", "image/upload/q_auto:eco"}}){:width="100%"}
{% endif %}
{% endfor %}