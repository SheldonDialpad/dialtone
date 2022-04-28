---
layout: page
title: Z-Index
description: Utility classes for setting an element's z-index level.
---
<section class="d-stack16">
    <header class="d-stack2">
        {% header "h2", "Variables" %}
        {% paragraph %}When writing Less, you can set an element's z-index by using a variable ({% code %}@zi-{level}{% endcode %}). The table below lists the available variables, output, and a description for when they should be used.{% endparagraph %}
    </header>
    <table class="d-table">
        <thead>
            <tr>
                <th scope="col" class="d-w25p">Variable</th>
                <th scope="col">Output</th>
                <th scope="col">Description</th>
            </tr>
        </thead>
        <tbody>
            {% for i in z-index %}
            {% assign name = i.name %}
            {% assign description = i.description %}
            {% assign output = i.output %}
            <tr>
                <th scope="row" class="d-ff-mono d-fc-pink-500 d-fs12 d-fw-normal">@zi-{{ name }}</th>
                <td>{{ output }}</td>
                <td class="dialtone-table--sans">{{ description }}</td>
            </tr>
            {% endfor %}
        </tbody>
    </table>
</section>
<section class="d-stack16">
    <header class="d-stack2">
        {% header "h2", "Classes" %}
        {% paragraph %}Set an element's z-index by using a class ({% code %}.d-zi-{level}{% endcode %}>). These classes match up with the variables names listed above. The table below lists the available z-index levels, class names, and the CSS output.{% endparagraph %}
    </header>
    <table class="d-table">
        <thead>
            <tr>
                <th scope="col" class="d-w25p">Class</th>
                <th scope="col">Output</th>
            </tr>
        </thead>
        <tbody>
            {% for i in z-index %}
            {% assign name = i.name %}
            {% assign description = i.description %}
            {% assign output = i.output %}
            <tr>
                <th scope="row" class="d-ff-mono d-fc-purple d-fs12 d-fw-normal">.d-zi-{{ name }}</th>
                <td class="d-ff-mono d-fc-orange d-fs12">z-index: {{ output }};</td>
            </tr>
            {% endfor %}
        </tbody>
    </table>
</section>
