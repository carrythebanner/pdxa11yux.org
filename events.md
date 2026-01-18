---
layout: default
---

# Events

## Upcoming Events

<ul>
  {% for post in site.posts reversed %}
    <li>
      <a href="{{ post.url }}">{{ post.title }} — {{ post.date | date_to_string }}</a>
    </li>
  {% endfor %}
</ul>

<!-- Currently lists all events; TODO add filter so only to future events are listed here -->

<iframe class="calendar-embed" title="Google Calendar of PDX A11Y UX events" src="https://calendar.google.com/calendar/embed?src=8f7533a01bb0bf584d696701c7dab6b4e148b125adc7e06975d67d41f6c8d9aa%40group.calendar.google.com&ctz=America%2FLos_Angeles" width="800" height="600" frameborder="0" scrolling="no"></iframe>

[Subscribe to calendar (iCal feed)](webcal://calendar.google.com/calendar/ical/8f7533a01bb0bf584d696701c7dab6b4e148b125adc7e06975d67d41f6c8d9aa%40group.calendar.google.com/public/basic.ics){: rel="external"}

You can also find our events on Portland's community tech calendar, [Calagator]( https://calagator.org/events/search?query=a11y){: rel="external"}.


## Past Events

Archive of past events coming soon! In the meantime, refer to <a href="https://www.meetup.com/portland-accessibility-and-user-experience-meetup/events/?type=past" rel="external">past events on Meetup</a> or via the [calendar embed](#upcoming-events) above.
