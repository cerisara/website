---
layout: leaderboard
---

{%- assign sorted_scores = site.data.scores | sort: "score" | reverse %}

<table border="1">
<thead>
    <tr>
      <th>Name</th>
      <th>Score</th>
    </tr>
</thead>
  <tbody>
  {%- for score in sorted_scores %}
    <tr>
    <td>{{ score.name }}</td> <td> {{ score.score }}</td>
    </tr>
  {%- endfor %}
  </tbody>
</table>

