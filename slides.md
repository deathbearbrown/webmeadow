---
layout: page
title: Presentation Archive
permalink: /presentations/
subheader: header-sub4.jpg
---
<div class="home">
  <ul class="post-list">
    {% for post in site.posts %}
      <li>
				<img class="small-image" src="/images/presentations/{{ post.thumbnail }}">
				<div class="post-info">
	        <span class="post-meta">{{ post.date | date: "%b %-d, %Y" }}</span>
	        <h2>
	          <a class="post-link" href="{{ post.url | prepend: site.baseurl }}">{{ post.title }}</a>
	        </h2>
	      </div>
      </li>
    {% endfor %}
  </ul>

</div>
