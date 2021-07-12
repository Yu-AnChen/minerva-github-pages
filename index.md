---
stories:
- Story 1: before_ashlar
---


This site is a minimal example using Github Pages to host [Minerva stories](https://github.com/labsyspharm/minerva-story/wiki) generated using [Minerva Author](https://github.com/labsyspharm/minerva-author).

__Please read the [Github Pages usage limits](https://docs.github.com/en/pages/getting-started-with-github-pages/about-github-pages#usage-limits) before hosting your Minerva story JPEG and PNG images.__


## Minerva Stories

{% for story_hash in page.stories %}
    {% for story in story_hash %}
- [{{ story[0] }}]({{ site.baseurl }}/{{ story[1] }})
    {% endfor %}
{% endfor %}
