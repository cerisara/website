---
layout: leaderboard
---

We innovate benchmarking along multiple dimensions:

- **System vs. LLM evaluation**: nowadays, LLMs are rarely standalone components and are integrated with other software components. We evaluate here a complete system, typically a RAG system.
- **French vs. English**: LLMs are known to be biased towards USA's point of view; we propose a benchmark that is built from the ground up from the French point of view about local and worldwide news.
- **Dynamic benchmarking**: Every newly released benchmark gets overfitted within a few months after its release. We propose a dynamic benchmark that is updated every 6 months.


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

