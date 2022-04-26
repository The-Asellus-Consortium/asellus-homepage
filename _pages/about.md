---
layout: single
classes: wide
permalink: /about/ 
---

# The Asellus Consortium

These are the current members of The Asellus Consoritum. Our goal is to better connect the community of isopod researchers through  meetings and symposia, compile data-sources, protocols and basic knowledge on _Asellus aquaticus_, and to organize.  

The consortium is open to anyone - if you are interested in helping us, please get in touch with us at [asellus.consortium@gmail.com](mailto:asellus.consortium@gmail.com)

<div class="member-grid">

	{% for member in site.data.members %}

	<div itemscope.itemtype="https://schema.org/Person">
	
		<div class="member-content">

		<img src= " {{ member.avatar_path }}" alt="{{ member.name }}" >
		
		<h3> {{ member.name }} </h3>
		<p> {{ member.institute }} </p>

		<p> <a href="{{ member.website }}"> website </a> | <a href="https://twitter.com/{{ member.twitter }}"> twitter </a> </p>
		
		
		<div class="member-bio" itemprop="description">
			<p> {{ member.bio }} </p>
		</div>
		
		</div>
	</div>
{% endfor %}
	</div>
