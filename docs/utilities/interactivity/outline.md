---
title: Outline 
desc: Utilities for controlling an element's outline.
---

## Classes

<utility-class-table>
  <template #content>
    <tbody>
      <tr v-for="{ class: className, output } in outline">
        <th scope="row" class="d-ff-mono d-fc-purple d-fs12">.{{ className }}</th>
        <td class="d-ff-mono d-fc-orange d-fs12">{{ output }}</td>
      </tr>
    </tbody>
  </template>
</utility-class-table>

## Usage

Use `d-ol-{focusring|none}` to change an elements' outline.

<code-well-header class="d-fl-col5 d-flg8 d-fw-wrap d-p24 d-bgc-purple-100 d-bgo50 d-w100p d-hmn102" custom>
  <div class="d-fl-center d-p16 d-ba d-bc-purple-300 d-bgc-purple-100 d-fs12 d-ff-mono d-ol-focusring">
    .d-ol-focusring
  </div>
  <div class="d-fl-center d-p16 d-ba d-bc-purple-300 d-bgc-purple-100 d-fs12 d-ff-mono d-ol-none">
    .d-ol-none
  </div>
</code-well-header>

```html
<div class="d-ol-focusring">...</div>
<div class="d-ol-none">...</div>
```

<script setup>
  import { outline } from '@data/interactivity.json';
</script>