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


## Past Events

Archive of past events coming soon! In the meantime, refer to <a href="https://www.meetup.com/portland-accessibility-and-user-experience-meetup/events/?type=past" rel="external">past events on Meetup</a> or via the [calendar embed](#upcoming-events) above.
