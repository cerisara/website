{%- assign sorted_scores = site.data.scores | sort_by: "score" %}

<h2>Leaderboard</h2>
<ul>
  {%- for score in sorted_scores %}
    <li>{{ score.name }} - {{ score.score }}</li>
  {%- endfor %}
</ul>

