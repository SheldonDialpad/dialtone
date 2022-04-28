---
layout: page
title: Padding
description: Utilities for setting an element's interior spacing between child elements and the element's box edge.
---
<section class="d-stack16">
    <header class="d-stack2">
        {% header "h2", "Classes" %}
        {% paragraph %}Padding can be added to an element by using a utility class (i.e. {% code %}.d-p[#]{% endcode %}) or by using a directional class (i.e. {% code %}.d-p{t|r|b|l|y|x}[#]{% endcode %}).{% endparagraph %}
    </header>
    <div class="d-h464 d-of-y-scroll d-bb d-bc-black-200">
        <table class="d-table">
            <thead>
                <tr>
                    <th scope="col" class="d-w25p">Class</th>
                    <th scope="col">Output</th>
                </tr>
            </thead>
            {% assign dir = spacing.directions | split: ", "  %}
            {% for i in dir %}
                <tbody>
                    {% for value in spacing.values %}
                    {% assign val = value.value %}
                    {% assign output = value.output %}
                    <tr>
                        <th scope="row" class="d-ff-mono d-fc-purple d-fw-normal d-fs12">.d-p{% if i != "All" %}{{ i | slice: 0 }}{% endif %}{{ val }}</th>
                        <td class="d-ff-mono d-fc-orange-500 d-fs12">
                            {% if i == "y" %}
                                padding-top: {{ output }} !important;<br/>
                                padding-bottom: {{ output }} !important;
                            {% elsif i == "x" %}
                                padding-right: {{ output }} !important;<br/>
                                padding-left: {{ output }} !important;
                            {% else %}
                                padding{% if i != "All" %}-{{ i }}{% endif %}: {{ output }} !important;
                            {% endif %}
                        </td>
                    </tr>
                    {% endfor %}
                </tbody>
            {% endfor %}
            <tbody>
                {% assign dir = spacing.directions | split: ", "  %}
                {% for i in dir %}
                <tr>
                    <th scope="row" class="d-ff-mono d-fc-purple d-fw-normal d-fs12">.d-p{% if i != 'All' %}{{ i | slice: 0 }}{% endif %}-unset</th>
                    <td class="d-ff-mono d-fc-orange-500 d-fs12">
                        {% if i == "y" %}
                            padding-top: unset !important;<br/>
                            padding-bottom: unset !important;
                        {% elsif i == "x" %}
                            padding-right: unset !important;<br/>
                            padding-left: unset !important;
                        {% else %}
                            padding{% if i != "All" %}-{{ i }}{% endif %}: unset !important;
                        {% endif %}
                    </td>
                </tr>
                {% endfor %}
            </tbody>
        </table>
    </div>
</section>
<section class="d-stack16">
    {% header "h2", "Add padding to all sides" %}
    <aside class="d-bar8 d-of-hidden">
        <header class="d-fl-center d-p24 d-bgc-purple-100 d-bgo50 d-w100p d-hmn216">
            <div class="d-h128 d-w128 d-p16 d-bar8 d-bgc-purple-200 d-of-hidden"><div class="d-fl-center d-fl1 d-h100p d-bgc-purple-300 d-bar4 d-fs14 d-ff-mono">d-p16</div></div>
        </header>
        <footer class="d-p8 d-bgc-black-700 d-bbr8 d-fs12">
{% highlight html linenos %}
<div class="d-p8 ...">d-p8</div>
{% endhighlight %}
        </footer>
    </aside>
</section>
    <section class="d-stack16">
    {% header "h2", "Add padding to a single side" %}
    <aside class="d-bar8 d-of-hidden">
        <header class="d-d-flex d-fw-wrap d-ai-start d-jc-center d-bgc-green-100 d-bgo50 d-w100p d-hmn216 d-flow24">
            <div class="d-as-center d-pt12 d-bar8 d-bgc-green-300 d-of-hidden"><div class="d-fl-center d-p16 d-bgc-green-200 d-bbr4 d-fs14 d-ff-mono">d-pt12</div></div>
            <div class="d-as-center d-pr16 d-bar8 d-bgc-green-300 d-of-hidden"><div class="d-fl-center d-p16 d-bgc-green-200 d-brl4 d-fs14 d-ff-mono">d-pr16</div></div>
            <div class="d-as-center d-pb24 d-bar8 d-bgc-green-300 d-of-hidden"><div class="d-fl-center d-p16 d-bgc-green-200 d-btr4 d-fs14 d-ff-mono">d-pb24</div></div>
            <div class="d-as-center d-pl32 d-bar8 d-bgc-green-300 d-of-hidden"><div class="d-fl-center d-p16 d-bgc-green-200 d-brr4 d-fs14 d-ff-mono">d-pl32</div></div>
        </header>
        <footer class="d-p8 d-bgc-black-700 d-bbr8 d-fs12">
{% highlight html linenos %}
<div class="d-pt12 ...">d-pt12</div>
<div class="d-pr16 ...">d-pr16</div>
<div class="d-pb24 ...">d-pb24</div>
<div class="d-pl32 ...">d-pl32</div>
{% endhighlight %}
        </footer>
    </aside>
</section>
<section class="d-stack16">
    {% header "h2", "Add horizontal padding" %}
    <aside class="d-bar8 d-of-hidden">
        <header class="d-d-flex d-fw-wrap d-ai-start d-jc-center d-bgc-pink-100 d-bgo50 d-w100p d-hmn216">
            <div class="d-as-center d-px24 d-bar8 d-bgc-pink-300 d-of-hidden"><div class="d-fl-center d-p16 d-bgc-pink-200 d-fs14 d-ff-mono">d-px24</div></div>
        </header>
        <footer class="d-p8 d-bgc-black-700 d-bbr8 d-fs12">
{% highlight html linenos %}
<div class="d-px24 ...">d-px24</div>
{% endhighlight %}
        </footer>
    </aside>
</section>
<section class="d-stack16">
    {% header "h2", "Add vertical padding" %}
    <aside class="d-bar8 d-of-hidden">
        <header class="d-d-flex d-fw-wrap d-ai-start d-jc-center d-bgc-red-100 d-bgo50 d-w100p d-hmn216">
            <div class="d-as-center d-py24 d-bar8 d-bgc-red-300 d-of-hidden"><div class="d-fl-center d-p16 d-bgc-red-200 d-fs14 d-ff-mono">d-py24</div></div>
        </header>
        <footer class="d-p8 d-bgc-black-700 d-bbr8 d-fs12">
{% highlight html linenos %}
<div class="d-py24 ...">d-py24</div>
{% endhighlight %}
        </footer>
    </aside>
</section>
