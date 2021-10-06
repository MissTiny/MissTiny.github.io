---
layout: page
permalink: /teaching/
title: teaching
description: # Materials for courses you taught. Replace this text with your description.
nav: true
---
<div class="teachings">
    <table class="table table-hover">
    <thead>
        <tr>
        <th scope="col-2">Year</th>
        <th scope="col-2">Position</th>
        <th scope="col-3">Course/Topic</th>
        <th scope="col-3">Location</th>
        <th scope="col-4">Description</th>
        </tr>
    </thead>
    <tbody>
    {% assign sorted_teachings = site.teaching | sort: "year" | reverse %}
    {% for teaching in sorted_teachings %}
        <tr class="teaching" >
            <td class="col-2" style="vertical-align:middle">
                {{ teaching.time }}
            </td>
            <td class="col-2" style="vertical-align:middle">
                {{ teaching.position }}
            </td>
            <td class="col-3" style="vertical-align:middle">
                {{teaching.title}}
            </td>
            <td class="col-3" id="location" style="vertical-align:middle">
                {{teaching.location}}
            </td>
            <td class="col-4" id="description" style="vertical-align:middle" data-bs-toggle="tooltip" data-bs-placement="right" title="{{teaching.description}}">
                {% if teaching.redirect %}
                <a href="{{teaching.redirect}}" target="_blank">click to see more</a>
                {% else %}
                <a href="{{ teaching.url | relative_url }}"> click to see more</a>
                {% endif %}
            </td>
        </tr>
    {% endfor %}
    </tbody>
</table>
</div>