---
layout: page
title: Max-width
description: Utilities to control an element's maximum width.
---
<section class="d-stack16">
    {% header "h2", "Classes" %}
    <div class="d-h464 d-of-y-scroll d-bb d-bc-black-200">
        <table class="d-table">
            <thead>
                <tr>
                    <th scope="col" class="d-w30p">Class</th>
                    <th scope="col">Output</th>
                </tr>
            </thead>
            <tbody>
                {% assign percentages = width-height.percentage | split: ", " %}
                {% for i in percentages %}
                <tr>
                    <th scope="row" class="d-ff-mono d-fc-purple d-fw-normal d-fs12">.d-wmx{{ i }}p</th>
                    <td class="d-ff-mono d-fc-orange-500 d-fs12">max-width: {{ i }}% !important;</td>
                </tr>
                {% endfor %}
            </tbody>
            <tbody>
                {% assign fixed = width-height.fixed | split: ", " %}
                {% for i in fixed %}
                <tr>
                    <th scope="row" class="d-ff-mono d-fc-purple d-fw-normal d-fs12">.d-wmx{{ i }}</th>
                    <td class="d-ff-mono d-fc-orange-500 d-fs12">max-width: {{ i }}px !important;</td>
                </tr>
                {% endfor %}
            </tbody>
            <tbody>
                {% assign fixed = width-height.other | split: ", " %}
                {% for i in fixed %}
                <tr>
                    <th scope="row" class="d-ff-mono d-fc-purple d-fw-normal d-fs12">.d-wmx-{{ i }}</th>
                    <td class="d-ff-mono d-fc-orange-500 d-fs12">max-width: {{ i }} !important;</td>
                </tr>
                {% endfor %}
            </tbody>
        </table>
    </div>
</section>
<section class="d-stack16">
    <header class="d-stack2">
        {% header "h2", "Percentages" %}
        {% paragraph %}Use {% code %}d-wmx{n}p{% endcode %} to set a minimum width percentage for an element. This can be combined with {% code %}d-w{n}p{% endcode %} and {% code %}d-wmn{n}{% endcode %} to have an element fill a certain height range.{% endparagraph %}
    </header>
    <aside class="d-bar8 d-of-hidden">
        <header class="d-d-flex d-jc-center d-p24 d-bgc-purple-100 d-bgo50 d-w100p d-flow16">
            <div class="d-fl-center d-py16 d-px8 d-w100p d-wmx50p d-bgc-purple-300 d-bar4 d-fs24 d-fw-bold d-ta-center">1</div>
        </header>
        <footer class="d-p8 d-bgc-black-700 d-bbr8 d-fs12">
{% highlight html linenos %}
<div class="d-w100p d-wmx50p">1</div>
{% endhighlight %}
        </footer>
    </aside>
</section>
<section class="d-stack16">
    <header class="d-stack2">
        {% header "h2", "Fixed" %}
        {% paragraph %}Use {% code %}d-wmx{n}{% endcode %} to set a fixed minimum width for an element. This can be combined with {% code %}d-w{n}p{% endcode %} and {% code %}d-wmn{n}{% endcode %} to have an element fill a certain height range.{% endparagraph %}
    </header>
    <aside class="d-bar8 d-of-hidden">
        <header class="d-d-flex d-jc-center d-p24 d-bgc-pink-100 d-bgo50 d-w100p d-flow16 d-of-y-scroll">
            <div class="d-fl-center d-py16 d-px8 d-w100p d-h64 d-wmx64 d-bgc-pink-300 d-bar4 d-fs24 d-fw-bold d-ta-center">1</div>
            <div class="d-fl-center d-py16 d-px8 d-w100p d-h64 d-wmx96 d-bgc-pink-300 d-bar4 d-fs24 d-fw-bold d-ta-center">2</div>
            <div class="d-fl-center d-py16 d-px8 d-w100p d-h64 d-wmx332 d-bgc-pink-300 d-bar4 d-fs24 d-fw-bold d-ta-center">3</div>
        </header>
        <footer class="d-p8 d-bgc-black-700 d-bbr8 d-fs12">
{% highlight html linenos %}
<div class="d-w100p d-wmx64">1</div>
<div class="d-w100p d-wmx96">2</div>
<div class="d-w100p d-wmx332">3</div>
{% endhighlight %}
        </footer>
    </aside>
</section>
