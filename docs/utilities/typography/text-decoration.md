---
title: Text Decoration
desc: Utilities to change an element's text decoration styles.
---

## Classes
<utility-class-table>
  <template #content>
    <tbody>
      <tr v-for=" i in decoration">
        <th scope="row" class="d-ff-mono d-fc-purple d-fw-normal d-fs12">.d-td-{{ i }}</th>
        <td class="d-ff-mono d-fc-orange d-fs12">
          <span v-if="i === 'dotted'">text-decoration: underline {{ i }} !important</span>
          <span v-else>text-decoration: {{ i }} !important</span>
        </td>
      </tr>
    </tbody>
  </template>
</utility-class-table>

## Underline
Use `d-td-underline` to underline text.

<code-well-header class="d-d-flex d-jc-center d-fd-column d-p24 d-bgc-pink-100 d-w100p d-hmn102" custom>
  <p class="d-fs24 d-fc-pink d-td-underline">The quick brown fox jumps over the lazy dog.</p>
</code-well-header>

```html
<p class="d-td-underline">...</p>
```

## Dotted
Use `d-td-dotted` to apply a dotted underline style to the text.

<code-well-header class="d-d-flex d-jc-center d-fd-column d-p24 d-bgc-purple-100 d-w100p d-hmn102" custom>
  <p class="d-fs24 d-fc-purple d-td-dotted">The quick brown fox jumps over the lazy dog.</p>
</code-well-header>

```html
<p class="d-td-dotted">...</p>
```

## Line Through
Use `d-td-line-through` to apply a line through the text.

<code-well-header class="d-d-flex d-jc-center d-fd-column d-p24 d-bgc-green-100 d-w100p d-hmn102" custom>
  <p class="d-fs24 d-fc-green d-td-line-through">The quick brown fox jumps over the lazy dog.</p>
</code-well-header>

```html
<p class="d-td-line-through">...</p>
```

## No decorations
Use `d-td-none` to remove text decorations.

<code-well-header class="d-d-flex d-jc-center d-fd-column d-p24 d-bgc-red-100 d-w100p d-hmn102" custom>
            <p class="d-fs24 d-fc-red d-td-none">The quick brown fox jumps over the lazy dog.</p>
</code-well-header>

```html
<p class="d-td-none">...</p>
```

<script setup>
  import { decoration } from '@data/type.json';
</script>