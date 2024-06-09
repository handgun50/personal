---
layout: page
title: Family Farm Adventure
collection: ffa
---

{: .box-note}
I'm on chapter 3 right now. The game is fun for filling my day. Right now, I'm focusing on continuing chapter story. The events are quite hard to finish because it uses too many energies and the events are non-stop.

{% for row in site.data.images %}
{% if row["collection"] == page.collection %}
![{{row["caption"]}}]({{row["link"] | replace: "image/upload", "image/upload/q_auto:eco"}}){:width="100%"}
{% endif %}
{% endfor %}