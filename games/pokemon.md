---
layout: page
title: Pokemon
collection: pokemon
---

{: .box-note}
I played a lot of pokemon games. From Pokemon GBA (for example Pokemon Fire Red) until Pokemon NDS (for example Pokemon Black). But I haven't played Pokemon on 3DS and onwards. Sometimes I also played fan-made pokemon games like Pokemon Glazed. 

{% for row in site.data.images %}
{% if row["collection"] == page.collection %}
![{{row["caption"]}}]({{row["link"] | replace: "image/upload", "image/upload/q_auto:eco"}}){:width="100%"}
{% endif %}
{% endfor %}


