# {{page.title}}

{% if site.data.scholars.size > 0 %}

Game Devs of Color Expo is excited to partner with the Game Developers Conference! We're running a scholarship program to help bring some amazing creators of color to GDC. GDC can be a career-defining conference, but tickets, travel, and lodging prices can place it out of reach for many developers. We've provided Conference and Summits passes and financial assistance when needed to these amazing scholars!

<br/>

  <ul class="list-unstyled">
    {% assign sorted_scholars = site.data.scholars | sort:"title" %}
    {% for game in sorted_scholars %}
    <li class="list-data col-container">
      <div class="col-3">
        <a href="{{game.link}}" target="_blank">
          <img src="/assets/images/scholars/2019/{{game.image}}" class="list-data-photo">
        </a>
      </div>
      <div class="col-3-2">
        <a href="{{game.link}}" target="_blank">
          <h2 class="list-data-title">{{game.title}}</h2>
        </a>
        <h3 class="list-data-title">{{game.team}}</h3>
        {% if game.description %}
        <p class="list-data-description text-smaller">{{ game.description }}</p>
        {% endif %}
      </div>
    </li>
    {% endfor %}
  </ul>
  <br>

{% else %}

### We'll be announcing our 2019 GDC Scholars soon. Stay tuned!

{% endif %}

----

### Sponsor info

<ul class="col-container sponsors-container">
<li class="col-3">
<p>
<a href="http://www.capybaragames.com" target="_blank">
<img src="/assets/images/scholars/2019/CapybaraGames_logo.png">
</a>
</p>
</li>
<li class="col-3">
<p>
<br/>
<br/>
<a href="https://subsetgames.com/" target="_blank">
<img src="/assets/images/scholars/2019/SubsetGames_logo.png">
</a>
</p>
</li>
</ul>

<br/>

<h4>Wadjet Eye Games</h4>
<p>
Learn more <a href="http://www.wadjeteyegames.com/" target="_blank">on their website.</a>
</p>

----

### Scholarship committee info

----

Interesting in applying to our GDC Scholar Program next year? Sign up for our mailing list for news and announcements!

{% include mailchimp-form.html %}