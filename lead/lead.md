{%- assign sorted_scores = site.data.scores | sort: "score" | reverse %}

<div class="leaderboard">
<h2>Leaderboard</h2>
<ul>
  {%- for score in sorted_scores %}
    <li>{{ score.name }} - {{ score.score }}</li>
  {%- endfor %}
</ul>
</div>

