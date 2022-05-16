---
title: Font Family
desc: Utilities to change an element's font-family.
---

## CSS Variables
<table class="d-table">
  <thead>
    <tr>
      <th scope="col" class="d-w40p">Variable</th>
      <th scope="col">Output</th>
    </tr>
  </thead>
  <tbody>
    <tr v-for="{ var: varName, output } in fontFamily.slice(0, -1)">
      <td class="d-ff-mono d-fc-purple d-fw-normal d-fs12">var(--ff-{{ varName }})</td>
      <td class="d-ff-mono d-fc-orange d-fs12">{{ output }}</td>
    </tr>
  </tbody>
</table>

## Classes
<table class="d-table">
  <thead>
    <tr>
      <th scope="col" class="d-w40p">Class</th>
      <th scope="col">Output</th>
    </tr>
  </thead>
  <tbody>
    <tr v-for="{ var: varName, output } in fontFamily">
      <td class="d-ff-mono d-fc-purple d-fw-normal d-fs12">.d-ff-{{ varName }}</td>
      <td class="d-ff-mono d-fc-orange d-fs12">font-family: {{ output }} !important;</td>
    </tr>
  </tbody>
</table>

## Custom
Use `d-ff-custom` to apply the theme's font-family.

<code-well-header class="d-d-flex d-jc-center d-fd-column d-p24 d-bgc-black-050 d-w100p d-hmn102" custom>
  <p class="d-fs24 d-ff-custom">The quick brown fox jumps over the lazy dog.</p>
</code-well-header>

```html
<p class="d-ff-custom">...</p>
```

## Sans-serif
Use `d-ff-sans` to apply a Sans-Serif font stack.

<code-well-header class="d-d-flex d-jc-center d-fd-column d-p24 d-bgc-black-050 d-w100p d-hmn102" custom>
  <p class="d-fs24 d-ff-sans">The quick brown fox jumps over the lazy dog.</p>
</code-well-header>

```html
<p class="d-ff-sans">...</p>
```

## Mono
Use `d-ff-mono` to apply a Sans-Serif font stack.

<code-well-header class="d-d-flex d-jc-center d-fd-column d-p24 d-bgc-black-050 d-w100p d-hmn102" custom>
  <p class="d-fs24 d-ff-mono">The quick brown fox jumps over the lazy dog.</p>
</code-well-header>

```html
<p class="d-ff-mono">...</p>
```

## Marketing
Dialtone supports select marketing fonts and weights. Use the following combinations to apply the marketing font stack.

<code-well-header class="d-d-flex d-jc-center d-fd-column d-p24 d-bgc-black-050 d-w100p d-hmn102" custom>
  <p class="d-fs24 d-ff-marketing">The quick brown fox jumps over the lazy dog.</p>
</code-well-header>

```html
<p class="d-ff-marketing">...</p>
```

<code-well-header class="d-d-flex d-jc-center d-fd-column d-p24 d-bgc-black-050 d-w100p d-hmn102" custom>
  <p class="d-fs24 d-ff-marketing-semi-expanded">The quick brown fox jumps over the lazy dog.</p>
</code-well-header>

```html
<p class="d-ff-marketing-semi-expanded">...</p>
```

<code-well-header class="d-d-flex d-jc-center d-fd-column d-p24 d-bgc-black-050 d-w100p d-hmn102" custom>
  <p class="d-fs24 d-ff-marketing-expanded">The quick brown fox jumps over the lazy dog.</p>
</code-well-header>

```html
<p class="d-ff-marketing-expanded">...</p>
```

<script setup>
  import { fontFamily } from '@data/type.json';
</script>