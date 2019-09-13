---
layout: page
title: Coordination
permalink: /coordination/
sidebar_link: true
---

We are trying to keep project communications to this [Slack Channel](https://himbworkspace.slack.com).  
(Email <jmadin@hawaii.edu> to be added.)

### Next meeting: TBA

We will attempt to have all-hands meetings every 2-3 weeks open to everyone.

### Fieldwork coordinators

- [Shreya Yadav](mailto:shreyay@hawaii.edu)
- [Ty Roach](mailto:smokinroachjr@gmail.com)
- TBA (we have received funding to support a program dedicated researcher)

### Layer coordinators 

<table>
{% for layer in site.data.layers %}
    <tr><td>{{ layer.name }}</td><td>
    {% for link in site.data.coordination %}
      {% if link.layer == layer.name %}
        {% for person in site.data.people %}
          {% if link.name == person.name %}
          <a href="mailto:{{ person.email }}">
            {{ person.name }}
          </a> |
          {% endif %}
        {% endfor %}
      {% endif %}
    {% endfor %}
    </td></tr>
{% endfor %}
</table>

### Other coordination (in progress)

- Hawai‘i’s He‘eia National Estuarine Research Reserve (He‘eia NERR)
- HIMB outreach and education programs
- Hawai'i Monitoring and Reporting Collaborative (HIMARC)
- NOAA
- DAR
- Hawaiʻi Coral Bleaching Collaborative (HCBC)
- MarineGEO (Smithsonian)

Go to [Resources](/resources) for useful information about the project and bleaching event.
