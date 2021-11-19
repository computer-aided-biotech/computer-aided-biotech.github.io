---
# Feel free to add content and custom Front Matter to this file.
# To modify the layout, see https://jekyllrb.com/docs/themes/#overriding-theme-defaults

layout: home
---
<div class="card text-white bg-warning mb-3">
  <div class="card-header">Under construction</div>
  <div class="card-body">
    <!-- <h5 class="card-title">Under construction!</h5> -->
    <p class="card-text">This site will be finished soon! <img src="/assets/images/giphy.gif" height="80" alt="Responsive image"></p>
    
  </div>
</div>
<div class="jumbotron jumbotron-fluid">
  <div class="container">
    <h1 class="display-1 text-white">CAB group</h1>
    <p class="lead text-white">Models. Robots. Software.</p>
    <p class="lead text-center  ">
      <a class="btn btn-primary btn-lg" href="research" role="button">About us</a>
    </p>
  </div>
</div>

<div class="container">
  <div class="row">
    <div class="col-8">
      <h2>Welcome to our group!</h2>
      <p>Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua. Ut enim ad minim veniam, quis nostrud exercitation ullamco laboris nisi ut aliquip ex ea commodo consequat. Duis aute irure dolor in reprehenderit in voluptate velit esse cillum dolore eu fugiat nulla pariatur. Excepteur sint occaecat cupidatat non proident, sunt in culpa qui officia deserunt mollit anim id est laborum.</p>
      <h3>Latest news</h3>
      
        {% for post in site.posts %}
            <h5><span class="float-left text-muted text-small"> {{ post.date | date_to_long_string }}</span> > <a href="{{ post.url }}">{{ post.title }}</a></h5>
            {{ post.excerpt | strip_html | strip_newlines | truncate: 156 }}
        {% endfor %}
      
    </div>
    <div class="col-sm">
      {% twitter https://twitter.com/phantomas1234 maxwidth=500 limit=2 %}
    </div>
  </div>
</div>