---
layout: default
---

# Contact

## Email

Regular ol' [email](mailto:{{ site.email }}) is a great way to contact us!

You can also join our email list to receive periodic updates. You can join by any of these ways: 

* <a href="https://forms.gle/p3vrLkegef794MRB6" rel="external">Complete our email sign-up form</a> (uses Google Forms)
* RSVP to one of our <a href="https://www.eventbrite.com/o/portland-accessibility-and-user-experience-120639756036#events" rel="external">Eventbrite events</a> and opt in to receiving emails
* [Email us](mailto:{{ site.email }}?subject=Join%20email%20list) and ask to be added to the list

We only use emails for communicating about our group's activities and other local accessibility happenings. Your email is never shared with anyone else or used for another purpose.


## Connect

We connect with the community using a number of different sites and services. Connect, follow, or message us on any of these!

<ul>
{% for item in site.data.connect %}
  <li>
    <a href="{{ item.link }}" rel="external">{{ item.name }}</a>
  </li>
{% endfor %}
</ul>
