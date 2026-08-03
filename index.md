## About Me

Hi I’m Iptcyq. I code, make games and engineer random stuff on my laptop.

I just made this site because it’s the middle of exam season and I’m bored (and distracted). Which is also why it’s incomplete… I’ll get back to updating this eventually?

---

## Project Log

Completed projects with the occasional write-up.

{% assign posts = site.pages | where: "home_post", true | sort: "date" | reverse %}
{% for post in posts %}

{% if post.page_url %}
### [{{ post.title }}]({{ post.page_url | relative_url }})
{% else %}
### {{ post.title }}
{% endif %}

<small>{{ post.date | date: "%B %Y" }}{% if post.badge and post.external_url %} · <a href="{{ post.external_url }}">{{ post.badge }}</a>{% endif %}</small>


{{ post.summary }}

{% if post.thumbnail %}
<img src="{{ post.thumbnail }}" class="project-image"/>
{% endif %}

{% if post.video %}
<video width="640" controls class="project-video">
    <source src="{{ post.video }}" type="video/mp4">
    Your browser does not support the video tag.
</video>
{% endif %}

---

{% endfor %}

## Work in Progress

Things I am currently working on.

{% assign wip_posts = site.data.home_posts.wip | sort: "date" | reverse %}
{% for post in wip_posts %}

{% if post.page_url %}
### [{{ post.title }}]({{ post.page_url | relative_url }})
{% else %}
### {{ post.title }}
{% endif %}

<small>{{ post.date | date: "%B %Y" }}{% if post.badge and post.external_url %} · <a href="{{ post.external_url }}">{{ post.badge }}</a>{% endif %}</small>


{{ post.summary }}

{% if post.thumbnail %}
<img src="{{ post.thumbnail }}" class="project-image"/>
{% endif %}

{% if post.video %}
<video width="640" controls class="project-video">
    <source src="{{ post.video }}" type="video/mp4">
    Your browser does not support the video tag.
</video>
{% endif %}

---

{% endfor %}

## Archive

Incomplete projects that I might continue in the future.

{% assign archive_posts = site.data.home_posts.archive | sort: "date" | reverse %}
{% for post in archive_posts %}

{% if post.page_url %}
### [{{ post.title }}]({{ post.page_url | relative_url }})
{% else %}
### {{ post.title }}
{% endif %}

<small>{{ post.date | date: "%B %Y" }}{% if post.badge and post.external_url %} · <a href="{{ post.external_url }}">{{ post.badge }}</a>{% endif %}</small>


{{ post.summary }}

{% if post.thumbnail %}
<img src="{{ post.thumbnail }}" class="project-image"/>
{% endif %}

{% if post.video %}
<video width="640" controls class="project-video">
    <source src="{{ post.video }}" type="video/mp4">
    Your browser does not support the video tag.
</video>
{% endif %}

---

{% endfor %}



<p align="center">
<sub>
Last updated {{ site.time | date: "%B %Y" }}
</sub>
</p>