# {{page.title}}

Our 2017 arcade hosted a variety of games from around the world. Below are the {{site.data.2017.games.size}} of the games we had the pleasure of hosting.

<ul class="list-unstyled">
  {% assign sorted_games = site.data.2017.games | sort:"title" %}
  {% for game in sorted_games %}
  <li class="list-data col-container">
    <div class="col-3">
      <a href="{{game.link}}" target="_blank">
        <img src="/assets/images/games/2017/{{game.image}}" class="list-data-photo">
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

# {{page.title}}