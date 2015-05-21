---
---

A club full of lawyers who also have GitHub accounts.

Proving this diagram wrong since 2009:

![Github-Lawyer Venn Diagram](http://philarcher.org/diary/2012/policygit/venn1.png)

All you have to do to join is create a [pull request](https://github.com/dpp/lawyersongithub) with
information about your bar membership.

Here are the members:

<div class="lawyers">
{% assign lawyers = site.lawyers | where:"type","lawyer" %}
{% for lawyer in lawyers %}
  {% include lawyer.html lawyer=lawyer %}
{% endfor %}
</div>

<h2>Lawyers <em>at</em> GitHub</h2>
{% assign lawyers = site.lawyers | where:"type","githubber" %}
{% for lawyer in lawyers %}
  {% include lawyer.html lawyer=lawyer %}
{% endfor %}

<h2>Law students on GitHub</h2>
{% assign lawyers = site.lawyers | where:"type","student" %}
{% for lawyer in lawyers %}
  {% include lawyer.html lawyer=lawyer %}
{% endfor %}
