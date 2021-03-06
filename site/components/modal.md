---
layout: default
title: "Modal"
---

# Modal
- [Basic](#basic)
- [Sizes](#sizes)

## Basic
To **hide** the modal, just add the `.is-hidden` state class on the `.modal-container` wrapper.

<button class="btn btn--primary js-modal-trigger u-mb-15" data-target="exampleModal">Launch modal</button>

<div id="exampleModal" class="modal-container is-hidden">
  <section class="modal">
    <header class="modal__header">
      <h4 class="modal__title">Modal Title</h4>
      <a role="button" class="modal__close js-modal-close">
        <i class="i-remove"></i>
      </a>
    </header>
    <div class="modal__body">
        "You have your way. I have my way. As for the right way, the correct way, and the only way, it does not exist."
    </div>
    <footer class="modal__footer">
        <button type="button" class="btn js-modal-close">Close</button>
        <button type="button" class="btn btn--primary">Ok</button>
    </footer>
  </section>
</div>

```html
<body>
  <div id="exampleModal" class="modal-container">
    <section class="modal">
      <header class="modal__header">
        <h4 class="modal__title">Modal Title</h4>
        <a role="button" class="modal__close">
          <i class="i-remove"></i>
        </a>
      </header>
      <div class="modal__body">
          "You have your way. I have my way. As for the right way, the correct way, and the only way, it does not exist."
      </div>
      <footer class="modal__footer">
          <button type="button" class="btn">Close</button>
          <button type="button" class="btn btn--primary">Ok</button>
      </footer>
    </section>
  </div>

  <div class="mask"></div>
</div>
```

<div class="note note--warning u-mt-40">
Point does <strong>not</strong> include any JavaScript interaction with <strong>Modal</strong>. You need to implement the class toggle yourself.
</div>

## Sizes
Add `.modal--sm` or `.modal--lg` modifier class on `.modal` element to quickly change the size of modal content.

<div class="u-mb-15">
  <button class="u-mb-5 btn btn--primary js-modal-trigger" data-target="smModal">Small Modal</button>
  <button class="u-mb-5 btn btn--primary js-modal-trigger" data-target="lgModal">Large Modal</button>
</div>

<div id="smModal" class="modal-container is-hidden">
  <section class="modal modal--sm">
    <header class="modal__header">
      <h4 class="modal__title">Large Modal</h4>
      <a role="button" class="modal__close js-modal-close">
        <i class="i-remove"></i>
      </a>
    </header>
    <div class="modal__body">
      Nullam id dolor id nibh ultricies vehicula ut id elit. Duis mollis, est
      non commodo luctus, nisi erat porttitor ligula, eget lacinia odio sem
      nec elit. Sed posuere consectetur est at lobortis. Aenean lacinia
      bibendum nulla sed consectetur. Integer posuere erat a ante venenatis
      dapibus posuere velit aliquet. Aenean lacinia bibendum nulla sed
      consectetur.
    </div>
    <footer class="modal__footer">
        <button type="button" class="btn js-modal-close">Close</button>
        <button type="button" class="btn btn--primary">Ok</button>
    </footer>
  </section>
</div>

<div id="lgModal" class="modal-container is-hidden">
  <section class="modal modal--lg">
    <header class="modal__header">
      <h4 class="modal__title">Large Modal</h4>
      <a role="button" class="modal__close js-modal-close">
        <i class="i-remove"></i>
      </a>
    </header>
    <div class="modal__body">
      Nullam id dolor id nibh ultricies vehicula ut id elit. Duis mollis, est
      non commodo luctus, nisi erat porttitor ligula, eget lacinia odio sem
      nec elit. Sed posuere consectetur est at lobortis. Aenean lacinia
      bibendum nulla sed consectetur. Integer posuere erat a ante venenatis
      dapibus posuere velit aliquet. Aenean lacinia bibendum nulla sed
      consectetur.
    </div>
    <footer class="modal__footer">
        <button type="button" class="btn js-modal-close">Close</button>
        <button type="button" class="btn btn--primary">Ok</button>
    </footer>
  </section>
</div>

```html
<div id="smModal" class="modal-container">
  <section class="modal modal--sm">
    ...
  </section>
</div>

<div id="lgModal" class="modal-container">
  <section class="modal modal--lg">
    ...
  </section>
</div>
```
