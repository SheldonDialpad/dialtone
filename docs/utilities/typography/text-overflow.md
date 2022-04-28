---
layout: page
title: Text Overflow
description: Utilities for controlling an element's text overflow.
---
<section class="d-stack16">
    {% header "h2", "Classes" %}
    <table class="d-table">
        <thead>
            <tr>
                <th scope="col" class="d-w25p">Class</th>
                <th scope="col">Output</th>
            </tr>
        </thead>
        <tbody>
            <tr>
                <th scope="row" class="d-ff-mono d-fc-purple d-fw-normal d-fs12">.d-truncate</th>
                <td class="d-ff-mono d-fc-orange d-fs12">
                    overflow: hidden !important;<br/>
                    text-overflow: ellipsis !important;<br/>
                    white-space: nowrap !important;
                </td>
            </tr>
            {% assign overflow = "ellipsis, clip, unset" | split: ", " %}
            {% for i in overflow %}
                <tr>
                    <th scope="row" class="d-ff-mono d-fc-purple d-fw-normal d-fs12">.d-to-{{ i }}</th>
                    <td class="d-ff-mono d-fc-orange d-fs12">text-overflow: {{ i }} !important;</td>
                </tr>
            {% endfor %}
        </tbody>
    </table>
</section>
<section class="d-stack16">
    <header class="d-stack2">
        {% header "h2", "Truncate" %}
        {% paragraph %}Use {% code %}d-truncate{% endcode %} to truncate an element's text.{% endparagraph %}
    </header>
    <aside class="d-bar8 d-of-hidden">
        <header class="d-fl-center d-p24 d-bgc-green-100 d-bgo50 d-w100p d-hmn102">
            <div class="d-bgc-green-200 d-py8 d-px16 d-bar8 d-w332">
                <p class="d-fs18 d-truncate">Lorem ipsum dolor sit amet, consectetur adipisicing elit. Blanditiisitaquequodpraesentiumexplicaboincidunt? Dolores beatae nam at sed dolorum ratione dolorem nisi velit dolor.</p>
            </div>
        </header>
        <footer class="d-p8 d-bgc-black-700 d-bbr8 d-fs12">
{% highlight html linenos %}
<p class="d-truncate">...</p>
{% endhighlight %}
        </footer>
    </aside>
</section>
<section class="d-stack16">
    <header class="d-stack2">
        {% header "h2", "Ellipsis" %}
        {% paragraph %}Use {% code %}d-to-ellipsis{% endcode %} to truncate an element's overflowing text with an ellipsis ({% code %}...{% endcode %}) if needed.{% endparagraph %}
    </header>
    <aside class="d-bar8 d-of-hidden">
        <header class="d-fl-center d-p24 d-bgc-pink-100 d-bgo50 d-w100p d-hmn102">
            <div class="d-bgc-pink-200 d-py8 d-px16 d-bar8 d-w332">
                <p class="d-fs18 d-of-hidden d-to-ellipsis">Lorem ipsum dolor sit amet, consectetur adipisicing elit. Blanditiisitaquequodpraesentiumexplicaboincidunt? Dolores beatae nam at sed dolorum ratione dolorem nisi velit dolor.</p>
            </div>
        </header>
        <footer class="d-p8 d-bgc-black-700 d-bbr8 d-fs12">
{% highlight html linenos %}
<p class="d-of-hidden d-to-ellipsis">...</p>
{% endhighlight %}
        </footer>
    </aside>
</section>
<section class="d-stack16">
    <header class="d-stack2">
        {% header "h2", "Clip" %}
        {% paragraph %}Use {% code %}d-to-clip{% endcode %} to clip an element's overflowing text if needed.{% endparagraph %}
    </header>
    <aside class="d-bar8 d-of-hidden">
        <header class="d-fl-center d-p24 d-bgc-purple-100 d-bgo50 d-w100p d-hmn102">
            <div class="d-bgc-purple-200 d-py8 d-px16 d-bar8 d-w332">
                <p class="d-fs18 d-of-hidden d-to-clip">Lorem ipsum dolor sit amet, consectetur adipisicing elit. Blanditiisitaquequodpraesentiumexplicaboincidunt? Dolores beatae nam at sed dolorum ratione dolorem nisi velit dolor.</p>
            </div>
        </header>
        <footer class="d-p8 d-bgc-black-700 d-bbr8 d-fs12">
{% highlight html linenos %}
<p class="d-of-hidden d-to-clip">...</p>
{% endhighlight %}
        </footer>
    </aside>
</section>
