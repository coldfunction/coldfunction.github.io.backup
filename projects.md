---
title: Projects
layout: page
group: navigation
---


<!-- iterate through all tags on the site --> 
  <!-- for each tag, create an anchor by using the tag name as an id --> 
  <div >  
   

    <ul> <!-- create the list of posts -->
      <!-- iterate through all the posts on the site --> 
      {% for post in site.posts %} 
        <!-- list only those which contain the current tag --> 


        {% for tag in post.tags %}
       	{% if tag == "projects" %}

            <li>
              <a href="#{{ post.title }}">{{ post.title }}</a>
            </li>


        {% endif %}
        {% endfor %}

      {% endfor %}
    </ul>

  </div>


<article class="post-container post-container--single">

{% for post in site.posts %} 

{% for tag in post.tags %}
       	{% if tag == "projects" %}


<div>
 <HR color="#000000" size="10" >
  <header class="post-header">
    <h1 class="post-title"><a name="{{ post.title }}">{{ post.title }}</a> </h1>
  </header>

  <section class="post">
    {{ post.content }}
  </section>
 

</div>


        {% endif %}
        {% endfor %}



{% endfor %}

</article>

