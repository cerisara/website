---
layout: leaderboard
---

{%- assign sorted_scores = site.data.scores | sort: "score" | reverse %}

<ul>
  {%- for score in sorted_scores %}
    <li>{{ score.name }} {{ score.score | right:4 }}</li>
  {%- endfor %}
</ul>

