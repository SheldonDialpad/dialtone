---
layout: page
title: Text Decoration
description: Utilities to change an element's text decoration styles.
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
            {% assign style = type.decoration | split: ", " %}
            {% for i in style %}
                <tr>
                    <th scope="row" class="d-ff-mono d-fc-purple d-fw-normal d-fs12">.d-td-{{ i }}</th>
                    <td class="d-ff-mono d-fc-orange d-fs12">text-decoration: {% if i == "dotted" %}underline {% endif %}{{ i }} !important;</td>
                </tr>
            {% endfor %}
        </tbody>
    </table>
</section>
<section class="d-stack16">
    <header class="d-stack2">
        {% header "h2", "Underline" %}
        {% paragraph %}Use {% code %}d-td-underline{% endcode %} to underline text.{% endparagraph %}
    </header>
    <aside class="d-bar8 d-of-hidden">
        <header class="d-d-flex d-jc-center d-fd-column d-p24 d-bgc-pink-100 d-w100p d-hmn102">
            <p class="d-fs24 d-fc-pink d-td-underline">The quick brown fox jumps over the lazy dog.</p>
        </header>
        <footer class="d-p8 d-bgc-black-700 d-bbr8 d-fs12">
{% highlight html linenos %}
<p class="d-td-underline">...</p>
{% endhighlight %}
        </footer>
    </aside>
</section>
<section class="d-stack16">
    <header class="d-stack2">
        {% header "h2", "Dotted" %}
        {% paragraph %}Use {% code %}d-td-dotted{% endcode %} to apply a dotted underline style to the text.{% endparagraph %}
    </header>
    <aside class="d-bar8 d-of-hidden">
        <header class="d-d-flex d-jc-center d-fd-column d-p24 d-bgc-purple-100 d-w100p d-hmn102">
            <p class="d-fs24 d-fc-purple d-td-dotted">The quick brown fox jumps over the lazy dog.</p>
        </header>
        <footer class="d-p8 d-bgc-black-700 d-bbr8 d-fs12">
{% highlight html linenos %}
<p class="d-td-dotted">...</p>
{% endhighlight %}
        </footer>
    </aside>
</section>
<section class="d-stack16">
    <header class="d-stack2">
        {% header "h2", "Line Through" %}
        {% paragraph %}Use {% code %}d-td-line-through{% endcode %} to apply a line through the text.{% endparagraph %}
    </header>
    <aside class="d-bar8 d-of-hidden">
        <header class="d-d-flex d-jc-center d-fd-column d-p24 d-bgc-green-100 d-w100p d-hmn102">
            <p class="d-fs24 d-fc-green d-td-line-through">The quick brown fox jumps over the lazy dog.</p>
        </header>
        <footer class="d-p8 d-bgc-black-700 d-bbr8 d-fs12">
{% highlight html linenos %}
<p class="d-td-line-through">...</p>
{% endhighlight %}
        </footer>
    </aside>
</section>
<section class="d-stack16">
    <header class="d-stack2">
        {% header "h2", "No decorations" %}
        {% paragraph %}Use {% code %}d-td-none{% endcode %} to remove text decorations.{% endparagraph %}
    </header>
    <aside class="d-bar8 d-of-hidden">
        <header class="d-d-flex d-jc-center d-fd-column d-p24 d-bgc-red-100 d-w100p d-hmn102">
            <p class="d-fs24 d-fc-red d-td-none">The quick brown fox jumps over the lazy dog.</p>
        </header>
        <footer class="d-p8 d-bgc-black-700 d-bbr8 d-fs12">
{% highlight html linenos %}
<p class="d-td-none">...</p>
{% endhighlight %}
        </footer>
    </aside>
</section>
