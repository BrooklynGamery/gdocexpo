<!-- # {{page.title}}-->
Check out <a class="page-link" href="https://app.swapcard.com/event/2020-game-devs-of-color-expo/exhibitors/RXZlbnRWaWV3XzU4OTEz?">the full list of games on Swapcard.

<iframe src="https://app.swapcard.com/widget/event/2020-game-devs-of-color-expo/exhibitors/RXZlbnRWaWV3XzU4OTEz?showActions=true" style="border: none; margin: 0px; width: 100%; display: block; height: calc(100vh - 100px);"></iframe>

<!--

{% if site.data.games.size > 0 %}

Our arcade will host a variety of games from around the world. Below are {{site.data.games.size}} of the confirmed games you will be able to play when you attend the expo. More games are still being announced!


  <ul class="list-unstyled">
    {% assign sorted_games = site.data.games | sort:"title" %}
    {% for game in sorted_games %}
    <li class="list-data col-container">
      <div class="col-3">
{% if game.link %}
	  <a href="{{game.link}}" target="_blank">
  {% endif%}      
		<img src="/assets/images/games/2019/{{game.image}}" class="list-data-photo">
        
		{% if game.link %}
		</a>
		{% endif game.link %}
      </div>
      <div class="col-3-2">
{% if game.link %}
	  <a href="{{game.link}}" target="_blank">
  {% endif%} 
          <h2 class="list-data-title">{{game.title}}</h2>
		  {% if game.link %}
        </a>
		{% endif game.link %}
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

### Stay tuned for updates soon!

{% endif %}
-->
<!--
# Vendor tables

We will have tables available for companies that are interested hiring game developers of color and/or sharing their products with our unique demographic. Contact us at gdocexpo@gmail.com to learn more about pricing.

Want to do more? [Sponsor the event.](/sponsor)

{% if site.data.booths.size > 0 %}
  <ul class="list-unstyled">
    {% assign sorted_booths = site.data.booths | sort:"name" %}
    {% for booth in sorted_booths %}
    <li class="list-data col-container">
      <div class="col-3">
        <a href="{{booth.link}}" target="_blank">
          <img src="/assets/images/sponsors/2019/{{booth.image}}" class="list-data-photo">
        </a>
      </div>
      <div class="col-3-2">
        <a href="{{booth.link}}" target="_blank">
          <h2 class="list-data-title">{{booth.name}}</h2>
        </a>
        {% if booth.description %}
        <p class="list-data-description text-smaller">{{ booth.description }}</p>
        {% endif %}
      </div>
    </li>
    {% endfor %}
  </ul>
 
{% endif %}
-->
----

Stay in the loop. Subscribe to hear updates about our annual event! We usually send emails less than once per week. Emails are infrequent.

{% include mailchimp-form.html %}