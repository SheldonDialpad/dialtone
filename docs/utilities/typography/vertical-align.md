---
title: Vertical Align
desc: Utilities for controlling an element's text transform.
---

## Classes
<utility-class-table>
  <template #content>
    <tbody>
      <tr v-for="i in ['baseline', 'top', 'bottom', 'text-top', 'text-bottom', 'middle', 'sub', 'super', 'unset']">
          <th scope="row" class="d-ff-mono d-fc-purple d-fw-normal d-fs12">.d-va-{{ i }}</th>
          <td class="d-ff-mono d-fc-orange d-fs12">vertical-align: {{ i }} !important;</td>
      </tr>
    </tbody>
  </template>
</utility-class-table>

## Baseline
Use `d-va-baseline` to vertically align an element to the baseline.

<code-well-header class="d-px64 d-py32 d-bgc-green-100 d-bgo50 d-w100p" custom>
  <div class="d-w100p d-ps-relative d-lh0">
    <div class="d-w0 d-h32 d-d-inline-block d-va-baseline">
      <span class="d-ps-absolute d-t0 d-h32 d-w100p d-by d-bts-dashed d-bbs-dashed d-bc-green-400"></span>
      <span class="d-ps-absolute d-t0 d-h16 d-w100p d-by d-bts-dashed d-bbs-dashed d-bc-green-400"></span>
    </div>
    <p class="d-d-inline-block d-ps-relative d-zi-base1 d-fc-green-500 d-fs18">The quick brown fox jumps over the lazy dog.</p>
  </div>
</code-well-header>

```html
<div class="d-d-inline-block d-va-baseline">...</div>
```

## Top
Use `d-va-top` to vertically align an element to the top.

<code-well-header class="d-px64 d-py32 d-bgc-purple-100 d-bgo50 d-w100p" custom>
  <div class="d-w100p d-ps-relative d-lh0">
    <div class="d-w0 d-h32 d-d-inline-block d-va-top">
      <span class="d-ps-absolute d-t0 d-h32 d-w100p d-by d-bts-dashed d-bbs-dashed d-bc-purple-300"></span>
      <span class="d-ps-absolute d-t0 d-h16 d-w100p d-by d-bts-dashed d-bbs-dashed d-bc-purple-300"></span>
    </div>
    <p class="d-d-inline-block d-ps-relative d-zi-base1 d-fc-purple-400 d-fs18">The quick brown fox jumps over the lazy dog.</p>
  </div>
</code-well-header>

```html
<div class="d-d-inline-block d-va-top">...</div>
```

## Middle
Use `d-va-middle` to vertically align an element to middle.

<code-well-header class="d-px64 d-py32 d-bgc-pink-100 d-bgo50 d-w100p" custom>
  <div class="d-w100p d-ps-relative d-lh0">
    <div class="d-w0 d-h32 d-d-inline-block d-va-middle">
      <span class="d-ps-absolute d-t0 d-h32 d-w100p d-by d-bts-dashed d-bbs-dashed d-bc-pink-400"></span>
      <span class="d-ps-absolute d-t0 d-h16 d-w100p d-by d-bts-dashed d-bbs-dashed d-bc-pink-400"></span>
    </div>
    <p class="d-d-inline-block d-ps-relative d-zi-base1 d-fc-pink-500 d-fs18">The quick brown fox jumps over the lazy dog.</p>
  </div>
</code-well-header>

```html
<div class="d-d-inline-block d-va-middle">...</div>
```

## Bottom
Use `d-va-bottom` to vertically align an element to the bottom.

<code-well-header class="d-px64 d-py32 d-bgc-pink-100 d-bgo50 d-w100p" custom>
  <div class="d-w100p d-ps-relative d-lh0">
    <div class="d-w0 d-h32 d-d-inline-block d-va-bottom" style="height: 3rem;">
      <span class="d-ps-absolute d-t0 d-h32 d-w100p d-by d-bts-dashed d-bbs-dashed d-bc-pink-400"></span>
      <span class="d-ps-absolute d-t0 d-h16 d-w100p d-by d-bts-dashed d-bbs-dashed d-bc-pink-400"></span>
    </div>
    <p class="d-d-inline-block d-ps-relative d-zi-base1 d-fc-pink d-fs18">The quick brown fox jumps over the lazy dog.</p>
  </div>
</code-well-header>

```html
<div class="d-d-inline-block d-va-bottom">...</div>
```

## Text Top
Use `d-va-text-top` to vertically align an element to text top.

<code-well-header class="d-px64 d-py32 d-bgc-yellow-100 d-bgo50 d-w100p" custom>
  <div class="d-ps-relative d-lh0">
    <div class="d-w0 d-h32 d-d-inline-block d-va-text-top">
      <span class="d-ps-absolute d-t0 d-h32 d-w100p d-by d-bts-dashed d-bbs-dashed d-bc-yellow-500"></span>
      <span class="d-ps-absolute d-t0 d-h16 d-w100p d-by d-bts-dashed d-bbs-dashed d-bc-yellow-500"></span>
    </div>
    <p class="d-d-inline-block d-ps-relative d-zi-base1 d-fc-yellow d-fs18">The quick brown fox jumps over the lazy dog.</p>
  </div>
</code-well-header>

```html
<div class="d-d-inline-block d-va-text-top">...</div>
```

## Text Bottom
Use `d-va-text-bottom` to vertically align an element to text bottom.

<code-well-header class="d-px64 d-py32 d-bgc-red-100 d-bgo50 d-w100p" custom>
  <div class="d-w100p d-ps-relative d-lh0">
    <div class="d-w0 d-h32 d-d-inline-block d-va-text-bottom">
      <span class="d-ps-absolute d-t0 d-h32 d-w100p d-by d-bts-dashed d-bbs-dashed d-bc-red-400"></span>
      <span class="d-ps-absolute d-t0 d-h16 d-w100p d-by d-bts-dashed d-bbs-dashed d-bc-red-400"></span>
    </div>
    <p class="d-d-inline-block d-ps-relative d-zi-base1 d-fc-red d-fs18">The quick brown fox jumps over the lazy dog.</p>
  </div>
</code-well-header>

```html
<div class="d-d-inline-block d-va-text-bottom">...</div>
```