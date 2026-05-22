---
title: Resources
layout: default
---

<div>
<h2>DSSF Program Resources</h2>
<ul>
    {% for resource in site.resources %}

    <li><a href="{{ resource.url | relative_url }}">
        {{ resource.title }}
    </a></li>

    {% endfor %}
</ul>
</div>

## Other

- [Expectations and Procedures]({{ site.baseurl }}/expectations)
- [Digital Scholarship @ Bryn Mawr](https://digitalscholarship.blogs.brynmawr.edu/)
- [AskAthena Knowledge Base](https://askathena.brynmawr.edu/help)
