---
layout: page
title: Margins
description: Utilities to adjust an element's exterior spacing between other objects.
---
<section class="d-stack16">
    <header class="d-stack2">
        {% header "h2", "Classes" %}
        <div class="d-stack16">
          {% paragraph %}Margins can be added to an element by using a utility class (i.e. {% code %}.d-m[#]{% endcode %}) or by using a directional class (i.e. {% code %}.d-m{t|r|b|l|y|x}[#]{% endcode %}).{% endparagraph %}
          {% paragraph %}The margin utility classes help visually separate elements. Because layouts are highly contextual, margins are never applied natively to a component's outer wrapper. Instead you can use these margin classes to provide that space or the <a href="/utilities/layout/stacks/" class="d-link">Stack and Flow layouts</a>.{% endparagraph %}
        </div>
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
                        <th scope="row" class="d-ff-mono d-fc-purple d-fw-normal d-fs12">.d-m{% if i != "All" %}{{ i | slice: 0 }}{% endif %}{{ val }}</th>
                        <td class="d-ff-mono d-fc-orange-500 d-fs12">
                            {% if i == "y" %}
                                margin-top: {{ output }} !important;<br/>
                                margin-bottom: {{ output }} !important;
                            {% elsif i == "x" %}
                                margin-right: {{ output }} !important;<br/>
                                margin-left: {{ output }} !important;
                            {% else %}
                                margin{% if i != "All" %}-{{ i }}{% endif %}: {{ output }} !important;
                            {% endif %}
                        </td>
                    </tr>
                    {% endfor %}
                </tbody>
            {% endfor %}
            {% for i in dir %}
                <tbody>
                    {% for value in spacing.values %}
                    {% assign val = value.value %}
                    {% assign output = value.output %}
                    <tr>
                        <th scope="row" class="d-ff-mono d-fc-purple d-fw-normal d-fs12">.d-m{% if i != "All" %}{{ i | slice: 0 }}{% endif %}n{{ val }}</th>
                        <td class="d-ff-mono d-fc-orange-500 d-fs12">
                            {% if i == "y" %}
                                margin-top: -{{ output }} !important;<br/>
                                margin-bottom: -{{ output }} !important;
                            {% elsif i == "x" %}
                                margin-right: -{{ output }} !important;<br/>
                                margin-left: -{{ output }} !important;
                            {% else %}
                                margin{% if i != "All" %}-{{ i }}{% endif %}: -{{ output }} !important;
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
                    <th scope="row" class="d-ff-mono d-fc-purple d-fw-normal d-fs12">.d-m{% if i != 'All' %}{{ i | slice: 0 }}{% endif %}-auto</th>
                    <td class="d-ff-mono d-fc-orange-500 d-fs12">
                        {% if i == "y" %}
                            margin-top: auto !important;<br/>
                            margin-bottom: auto !important;
                        {% elsif i == "x" %}
                            margin-right: auto !important;<br/>
                            margin-left: auto !important;
                        {% else %}
                            margin{% if i != "All" %}-{{ i }}{% endif %}: auto !important;
                        {% endif %}
                    </td>
                </tr>
                {% endfor %}
            </tbody>
            <tbody>
                {% assign dir = spacing.directions | split: ", "  %}
                {% for i in dir %}
                <tr>
                    <th scope="row" class="d-ff-mono d-fc-purple d-fw-normal d-fs12">.d-m{% if i != 'All' %}{{ i | slice: 0 }}{% endif %}-unset</th>
                    <td class="d-ff-mono d-fc-orange-500 d-fs12">
                        {% if i == "y" %}
                            margin-top: unset !important;<br/>
                            margin-bottom: unset !important;
                        {% elsif i == "x" %}
                            margin-right: unset !important;<br/>
                            margin-left: unset !important;
                        {% else %}
                            margin{% if i != "All" %}-{{ i }}{% endif %}: unset !important;
                        {% endif %}
                    </td>
                </tr>
                {% endfor %}
            </tbody>
        </table>
    </div>
</section>
<section class="d-stack16">
    {% header "h2", "Add margin to all sides" %}
    <aside class="d-bar8 d-of-hidden">
        <header class="d-fl-center d-p24 d-bgc-purple-100 d-bgo50 d-w100p d-hmn216">
            <div class="d-bgc-purple-200 d-of-hidden"><div class="d-fl-center d-p16 d-m24 d-bgc-purple-300 d-bar4 d-fs14 d-ff-mono">d-m24</div></div>
        </header>
        <footer class="d-p8 d-bgc-black-700 d-bbr8 d-fs12">
{% highlight html linenos %}
<div class="d-m24 ...">d-m24</div>
{% endhighlight %}
        </footer>
    </aside>
</section>
<section class="d-stack16">
    {% header "h2", "Add margin to a single side" %}
    <aside class="d-bar8 d-of-hidden">
        <header class="d-d-flex d-fw-wrap d-ai-start d-jc-center d-bgc-green-100 d-bgo50 d-w100p d-hmn216 d-flow24">
            <div class="d-as-center d-bar8 d-bgc-green-200 d-of-hidden"><div class="d-fl-center d-mt12 d-p16 d-bgc-green-300 d-bbr4 d-fs14 d-ff-mono">d-mt12</div></div>
            <div class="d-as-center d-bar8 d-bgc-green-200 d-of-hidden"><div class="d-fl-center d-mr16 d-p16 d-bgc-green-300 d-brl4 d-fs14 d-ff-mono">d-mr16</div></div>
            <div class="d-as-center d-bar8 d-bgc-green-200 d-of-hidden"><div class="d-fl-center d-mb24 d-p16 d-bgc-green-300 d-btr4 d-fs14 d-ff-mono">d-mb24</div></div>
            <div class="d-as-center d-bar8 d-bgc-green-200 d-of-hidden"><div class="d-fl-center d-ml32 d-p16 d-bgc-green-300 d-brr4 d-fs14 d-ff-mono">d-ml32</div></div>
        </header>
        <footer class="d-p8 d-bgc-black-700 d-bbr8 d-fs12">
{% highlight html linenos %}
<div class="d-mt12 ...">d-mt12</div>
<div class="d-mr16 ...">d-mr16</div>
<div class="d-mb24 ...">d-mb24</div>
<div class="d-ml32 ...">d-ml32</div>
{% endhighlight %}
        </footer>
    </aside>
</section>
<section class="d-stack16">
    {% header "h2", "Add horizontal margins" %}
    <aside class="d-bar8 d-of-hidden">
        <header class="d-d-flex d-fw-wrap d-ai-start d-jc-center d-bgc-pink-100 d-bgo50 d-w100p d-hmn216">
            <div class="d-as-center d-bar8 d-bgc-pink-200 d-of-hidden"><div class="d-fl-center d-mx24 d-p16 d-bgc-pink-400 d-fs14 d-ff-mono">d-mx24</div></div>
        </header>
        <footer class="d-p8 d-bgc-black-700 d-bbr8 d-fs12">
{% highlight html linenos %}
<div class="d-mx24 ...">d-mx24</div>
{% endhighlight %}
        </footer>
    </aside>
</section>
<section class="d-stack16">
    {% header "h2", "Add vertical margins" %}
    <aside class="d-bar8 d-of-hidden">
        <header class="d-d-flex d-fw-wrap d-ai-start d-jc-center d-bgc-red-100 d-bgo50 d-w100p d-hmn216">
            <div class="d-as-center d-bar8 d-bgc-red-200 d-of-hidden"><div class="d-fl-center d-my24 d-p16 d-bgc-red-500 d-fs14 d-fc-white d-ff-mono">d-my24</div></div>
        </header>
        <footer class="d-p8 d-bgc-black-700 d-bbr8 d-fs12">
{% highlight html linenos %}
<div class="d-my24 ...">d-my24</div>
{% endhighlight %}
        </footer>
    </aside>
</section>
<section class="d-stack16">
    <header class="d-stack2">
        {% header "h2", "Auto margins" %}
        {% paragraph %}Auto margins allow an element to fill a remaining space within an object. This is especially useful in flex layouts.{% endparagraph %}
    </header>
    <aside class="d-bar8 d-of-hidden">
        <header class="d-bgc-yellow-100 d-bgo50 d-w100p d-hmn216 d-p24 d-stack16">
            <div class="d-d-flex d-bar8 d-bgc-yellow-200 d-of-hidden"><div class="d-fl-center d-mx-auto d-p16 d-bgc-yellow-400 d-fs14 d-ff-mono">d-mx-auto</div></div>
            <div class="d-d-flex d-bar8 d-bgc-yellow-200 d-of-hidden"><div class="d-fl-center d-ml-auto d-p16 d-bgc-yellow-400 d-fs14 d-ff-mono">d-ml-auto</div></div>
            <div class="d-d-flex d-bar8 d-bgc-yellow-200 d-of-hidden"><div class="d-fl-center d-mr-auto d-p16 d-bgc-yellow-400 d-fs14 d-ff-mono">d-mr-auto</div></div>
        </header>
        <footer class="d-p8 d-bgc-black-700 d-bbr8 d-fs12">
{% highlight html linenos %}
<div class="d-mx-auto ...">d-mx-auto</div>
<div class="d-ml-auto ...">d-ml-auto</div>
<div class="d-mr-auto ...">d-mr-auto</div>
{% endhighlight %}
        </footer>
    </aside>
</section>
