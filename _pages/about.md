---
layout: about
title: about
permalink: /
description: <a href="#">Affiliations</a>. Address. Contacts. Moto. Etc.

profile:
  align: right
  image: 
  address: >
 

news: false  # includes a list of news items
selected_papers: false # includes a list of papers marked as "selected={true}"
social: false  # includes social icons at the bottom of the page
---

---
layout: default
pagination:
  enabled: true
  collection: posts
  permalink: /page/:num/
  per_page: 3
  sort_field: date
  sort_reverse: true
  trail:
    before: 1 # The number of links before the current page
    after: 3  # The number of links after the current page
---

<div class="post">

  <div class="header-bar">
    <h1>{{ site.blog_name }}</h1>
    <h2>{{ site.blog_description }}</h2>
  </div>


  <ul class="post-list">
    {% for post in paginator.posts %}
      <li>
        <h3><a class="post-title" href="{{ post.url | prepend: site.baseurl }}">{{ post.title }}</a></h3>
        <p class="post-meta">{{ post.date | date: '%B %-d, %Y' }}</p>
        <p>{{ post.description }}</p>
      </li>
    {% endfor %}
  </ul>

  {% include pagination.html %}

</div>




Write your biography here. Tell the world about yourself. Link to your favorite [subreddit](http://reddit.com){:target="\_blank"}. You can put a picture in, too. The code is already in, just name your picture `prof_pic.jpg` and put it in the `img/` folder.

Put your address / P.O. box / other info right below your picture. You can also disable any these elements by editing `profile` property of the YAML header of your `_pages/about.md`. Edit `_bibliography/papers.bib` and Jekyll will render your [publications page](/al-folio/publications/) automatically.

Link to your social media connections, too. This theme is set up to use [Font Awesome icons](http://fortawesome.github.io/Font-Awesome/){:target="\_blank"} and [Academicons](https://jpswalsh.github.io/academicons/){:target="\_blank"}, like the ones below. Add your Facebook, Twitter, LinkedIn, Google Scholar, or just disable all of them.
