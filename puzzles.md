---
layout: page
title: Puzzles
permalink: /puzzles/
---
Here is a list of the puzzle descriptions we have made so far this term.

<table>
<thead>
    <tr>
        <th>Week</th>
        <th>Puzzle</th>
        <th>Solutions</th>
    </tr>
</thead>
<tbody>
{% for puzzle in site.puzzles %}
    {% unless puzzle.hide %}
    <tr>
        <td>Week {{puzzle.week}}</td>
        <td><a href="{{puzzle.url | prepend: site.baseurl}}">
            {{puzzle.title}}
        </a></td>
        <td>
        {% if puzzle.solutions %}
            <a href="https://github.com/D-HAC/solutions/tree/master/{{puzzle.solutions}}">
                Solutions
            </a>
        {% else %}
            Solutions Not Yet Available!
        {% endif %}
        </td>
    </tr>
    {% endunless %}
{% endfor %}
</tbody>
</table>
