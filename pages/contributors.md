---
layout: page
title: Contributors
permalink: "/contributors/"
<!--image: images/team/-->
---



<div class="container pt-6 pb-6">
    <div class="row">
    	{% for person in site.data.contributors %}
        <div class="col-12 col-md-6 mb-2">
            <div class="team team-summary team-summary-large">
                {% if person.image %}
                <div class="team-image">
                    <img width="90" height="90" alt="{{ team.title }}" class="img-fluid mb-2" src="{{ person.image | relative_url }}" />
                </div>
                {% endif %}
                <div class="team-meta">
                    <h2 class="team-name">{{ person.title }}</h2>
                    <p class="team-description">{{ person.jobtitle }}</p>
                    {% if person.linkedinurl %}
                    <h4 class="linkedinurl"><a target="_blank" href="{{ person.linkedinurl }}" rel="noreferrer">LinkedIn</a></h4>
                    {% endif %}
                    {% if person.github %}
                    <h4 class="github"><a target="_blank" href="{{ person.github }}" rel="noreferrer">Github</a></h4>
                    {% endif %}
                </div>
            </div>
        </div>
        {% endfor %}
    </div>
</div>

