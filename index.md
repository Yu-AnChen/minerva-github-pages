---
stories:
- Story 1: before_ashlar
---


This site is a minimal example using Github Pages to host [Minerva Stories](https://github.com/labsyspharm/minerva-story/wiki) generated using [Minerva Author](https://github.com/labsyspharm/minerva-author).

__Please read the [Github Pages usage limits](https://docs.github.com/en/pages/getting-started-with-github-pages/about-github-pages#usage-limits) before hosting your Minerva Story image and data files.__

If your files exceed the usage limits, please refer to [the instructions](https://github.com/labsyspharm/minerva-story/wiki/Hosting-Minerva-Story-on-GitHub) for migration to other file storage services.


## Minerva Stories

{% for story_hash in page.stories %}
    {% for story in story_hash %}
- [{{ story[0] }}]({{ site.baseurl }}/{{ story[1] }})
    {% endfor %}
{% endfor %}
