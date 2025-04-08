---
permalink: /projects/
title: My projects
projects:
    -
        name: crafting-calculator
        description: A calculator for what resources are required to build something
---
## Projects

<hr>

{%- for project in page.projects -%}
* [{{ project.name }}]({{ site.github.owner_url }}/{{ project.name }}): {{ project.description }}<br>
  [More information]({{ project.name }})
{%- endfor -%}
