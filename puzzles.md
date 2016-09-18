---
layout: page
title: Puzzles
permalink: /puzzles/
---
Here is a list of the puzzle descriptions we have made so far this term.

{% for puzzle in site.puzzles %}
{% unless puzzle.hide %}
[{{puzzle.title}}]({{puzzle.url | prepend: site.baseurl}})
{% endunless %}
{% endfor %}
