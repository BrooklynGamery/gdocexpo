# {{page.title}}

Our arcade will host a variety of games from around the world. Below are some of the games you will be able to play when you attend the expo.

<ul class="list-unstyled">
  {% assign sorted_games = site.data.games | sort:"title" %}
  {% for game in sorted_games %}
  <li class="list-data col-container">
    <div class="col-3">
      <img src="/assets/images/games/2017/{{game.image}}" class="list-data-photo">
    </div>
    <div class="col-3-2">
      <h2 class="list-data-title">{{game.title}}</h2>
      <h3 class="list-data-title">{{game.team}}</h3>
      {% if game.description %}
      <p class="list-data-description text-smaller">{{ game.description }}</p>
      {% endif %}
    </div>
  </li>
  {% endfor %}
</ul>

----

More information is coming soon. Subscribe to hear when we add new games, speakers, and more! We send emails less than once per week.

{% include mailchimp-form.html %}