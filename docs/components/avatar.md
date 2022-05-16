---
title: Avatar
desc: An avatar is a visual representation of a user or object.
storybook_url: https://vue.dialpad.design/?path=/story/components-avatar--default
prev:
  text: Utilities - Word break
  link: /utilities/typography/word-break
---

## Classes

<component-class-table component-name="avatar"></component-class-table>

## Examples

### Icons
<code-well-header>
    <div class="d-avatar d-avatar--md d-avatar--icon d-avatar--purple-600">
        <IconGroup/>
    </div>
</code-well-header>

```html
<div class="d-avatar d-avatar--icon d-avatar--purple-600">...</div>
```

### Images

<code-well-header>
    <div class="d-avatar d-avatar--md d-avatar--icon d-avatar--purple-600">
        <img src="/assets/images/person.png" alt=""/>
    </div>
</code-well-header>

```html
<div class="d-avatar d-avatar--{$size}">
    <img src="/path/to/image" />
</div>
```
### Initials

<code-well-header>
    <div class="d-w100p d-fl-col4 d-flg4 d-fw-wrap d-jc-space-between">
        <div v-for="color in colors" class="d-d-fl d-fl-center d-mb8">
            <div class="d-avatar d-avatar--md d-avatar--initials" :class="color">DP</div>
        </div>
    </div>
</code-well-header>

```html
<div class="d-avatar d-avatar--initials d-avatar--{$color} ...">DP</div>
```
### Sizes

<code-well-header>
    <div class="d-d-inline-flex d-ai-center d-flow8">
        <div class="d-avatar d-avatar--sm d-avatar--purple-600 d-avatar--initials d-mb8">DP</div>
        <div class="d-avatar d-avatar--md d-avatar--purple-600 d-avatar--initials d-mb8">DP</div>
        <div class="d-avatar d-avatar--lg d-avatar--purple-600 d-avatar--initials d-mb8">DP</div>
    </div>
</code-well-header>

```html
<div class="d-avatar d-avatar--sm ...">DP</div>
<div class="d-avatar d-avatar--md ...">DP</div>
<div class="d-avatar d-avatar--lg ...">DP</div>
```

## Accessibility

Initial avatars' background and font color combinations have been paired to ensure minimum contrast is met.

When it comes to voiceover, avatars accompanying a label should generally be considered decorative and shouldn't be
focusable or read out. An example is a user's avatar next to their name.

Avatars unaccompanied by labels, especially those representing functionality or navigation, should be focusable and
readout in voiceover. Please refer
to <a class="d-link" href="https://www.w3.org/WAI/tutorials/images/decorative/" target="_blank">WCAG</a> references for
your specific usage.

<script setup>
import IconGroup from "@svgIcons/IconGroup.vue";
import { colors } from '@data/avatar.json';
</script>