---
layout: default
---

# Events

## Upcoming Events

{% assign past_events   = site.posts | where_exp: "post", "post.date <= site.time" %}
{% assign future_events = site.posts | where_exp: "post", "post.date >  site.time" %}

<ul>
{% for post in future_events reversed %}
    <li>
      <a href="{{ post.url }}">{{ post.title }} — {{ post.date | date_to_string }}</a>
    </li>
{% else %}
    <li>
      No upcoming events — check back soon!
    </li>
{% endfor %}
</ul>

<iframe class="calendar-embed" title="Google Calendar of PDX A11Y UX events" src="https://calendar.google.com/calendar/embed?src=8f7533a01bb0bf584d696701c7dab6b4e148b125adc7e06975d67d41f6c8d9aa%40group.calendar.google.com&ctz=America%2FLos_Angeles" width="800" height="600" frameborder="0" scrolling="no"></iframe>

[Subscribe to calendar (iCal feed)](webcal://calendar.google.com/calendar/ical/8f7533a01bb0bf584d696701c7dab6b4e148b125adc7e06975d67d41f6c8d9aa%40group.calendar.google.com/public/basic.ics){: rel="external"}

You can also find our events on Portland's community tech calendar, [Calagator]( https://calagator.org/events/search?query=a11y){: rel="external"}.


## Past Events

Recent events:

<ul>
{% for post in past_events %}
    <li>
      <a href="{{ post.url }}">{{ post.title }} — {{ post.date | date_to_string }}</a>
    </li>
{% endfor %}
</ul>

Full archive of all past events coming soon! In the meantime, you can browse [past events on Meetup](https://www.meetup.com/portland-accessibility-and-user-experience-meetup/events/?type=past){: rel="external"} or in the [calendar embed](#upcoming-events) above.
