# Web Component Example

- A set of web platform APIs that allow you to create new custom, reusable, encapsulated HTML tags to use in web pages and web apps.
- Framework agnostic

## Web Component standards / Building blocks

- HTML Templates
- Shadow DOM
- Custom Elements

## Advantages

- CSS scoping
- DOM encapsulation
- Composition

---

### Shadow DOM

![Shadow Dom](https://developer.mozilla.org/en-US/docs/Web/Web_Components/Using_shadow_DOM/shadowdom.svg)

- A scoped subtree inside the element.
- Terminologies
  - Shadow host
  - Shadow tree
  - Shadow boundary
  - Shadow root

---

#### Go Through Shadow DOM

- Creating shadow DOM

```HTML
const header = document.createElement('header');
const shadowRoot = header.attachShadow({mode: 'open'});
shadowRoot.innerHTML = '<h1>Hello Shadow DOM</h1>';
```

- Composition and slots
  - `light DOM` and `shadow DOM`
  - `<slot>` element

```HTML
<!-- Default slot. If there's more than one default slot, the first is used. -->
<slot></slot>

<slot>fallback content</slot> <!-- default slot with fallback content -->

<slot> <!-- default slot entire DOM tree as fallback -->
  <h2>Title</h2>
  <summary>Description text</summary>
</slot>
```

- Styling

---

## References

- [Shadow DOM v1: Self-Contained Web Components](https://developers.google.com/web/fundamentals/web-components/shadowdom)
- [Using shadow DOM - Web Components | MDN](https://developer.mozilla.org/en-US/docs/Web/Web_Components/Using_shadow_DOM)
