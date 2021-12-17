# Devsign review checklist

A checklist that intends to help both sides: **_designers_** to prepare their mockups for implementation and **_developers_** to review them and ensure the quality of the implementation

## 1. Colors 🌈

- [ ] All the color variations used in mockups belong to the palette, they are named (`$dark-base`, `$dark-transparent-08`, `$success-base`) or accordingly to their use (`$color-text-primary`, `$color-overlay-background`, `$success-text-color`).
- [ ] Different color states of some elements (buttons, links, form inputs, ...) are defined and work in the context of light/dark/colored background or the rules of usage are documented.
- [ ] All of the most used color combinations are accessible and have sufficient contrast ratio.

:book: **Additional resources:**
- [Color and contrast accessibility](https://web.dev/color-and-contrast-accessibility/)
- [Contrast Checker](https://webaim.org/resources/contrastchecker/)
- [APCA contrast checker](https://www.myndex.com/APCA/simple)

## 2. Typography 🔠

- [ ] [Fallback font](https://en.wikipedia.org/wiki/Fallback_font) stack should be specified in the Style Guide along with the generic keyword.
- [ ] All the text styles used in mockups belong to the styleguide set of typography.<br>
      `font-size` + `line-height` _always_ must be paired to provide the legibility, readability and maintain vertical rhythm.
- [ ] As far as possible, all texts are provided in the proper language instead of dummy texts in English (Lorem Ipsum).

  > 💡 In the case of multilanguage content, think about how the layout can react if the content is longer than defined in the mockup.

:book: **Additional resources:**
- [Web font optimization](https://web.dev/fast/#optimize-webfonts)
- [CSS Basics: Fallback Font Stacks for More Robust Web Typography](https://css-tricks.com/css-basics-fallback-font-stacks-robust-web-typography/)
- [Rhythm in Typography | improve legibility, readability, and visual hierarchy](https://betterwebtype.com/articles/2018/10/15/rhythm-in-web-typography/)

## 3. Icons ♠️

- [ ] All icons are provided in SVG format, each _in the same square dimension_, in black color (`#000000`).
- [ ] All icons are named consistently and following the convention in lowercase using dashes to separate each word (e.g. `arrow-down.svg`, `icon-arrow-down.svg`)
- [ ] Before usage on the page all SVGs are optimized to get rid of unnecessary metadata and tags

:book: **Additional resources:**
- [SVGOMG - SVGO's Missing GUI](https://jakearchibald.github.io/svgomg/)

## 4.Grid system and spacing 📐
- [ ] A grid is explicitly provided in the design and and the details of the grid are present in the technical specification (width, gutters, number of columns, ...). All the elements follow the grid.
- [ ] All the spaces (margins, paddings, gutters) follow the defined grid. Their values should be limited to some set (e.g `4px, 8px, 16px, 24px, 32px, 40px, ...`, ).

  >❗️The box-model should be taken into account as the rendering in browser and in design tools are different

## 5. Links, buttons, navigation :link:
### 5.1. Links
- [ ] All the links have the following states clearly defined (the Style guide is the best document to specify this once and use consistenly):
    - default
    - hover (when mouseover)
    - focus (from keyboard, probably the global pattern)
    - active (when mousedown/pressed)
    - visited (if needed)
- [ ] All the links are designed in accessible and usable way.

:book: **Additional resources:**
- [Link contrast checker](https://webaim.org/resources/linkcontrastchecker/)

### 5.2. Buttons
- [ ] All the buttons have the following states clearly defined:
    - default
    - hover (when mouseover)
    - focus (from keyboard, probably the global pattern)
    - active (when mousedown/pressed)
    - disabled (when action is not available)
    - loading (if needed)

### 5.3 Navigation
- [ ] Alternate views of all navigation states are defined:
  - hover
  - focused (from keyboard, probably the global pattern)
  - active/current page

:book: **Additional resources:**
- [Proper Use of Buttons and Links](http://www.webaxe.org/proper-use-buttons-links/)
- [Button UX Design: Best Practices, Types and States – UX Planet](https://uxplanet.org/button-ux-design-best-practices-types-and-states-647cf4ae0fc6)
- [Buttons in Design Systems](https://medium.com/eightshapes-llc/buttons-in-design-systems-eac3acf7e23)

## Forms :ballot_box_with_check:
- [ ] All forms have title to provide basic instructions and context.
- [ ] All the form fields (inputs, selects, checkboxes, radio buttons, etc.) have the following states clearly defined (the Style guide is the best document to specify this once and use consistenly):
  - default
  - hover (when mouseover, if needed)
  - focus (when enter the data, from keyboard, probably the global pattern)
  - active (when mousedown/pressed, if needed)
  - disabled (when input is not available)
  - error state with a clear message
- [ ] Indicators of required/optional fields are provided.
- [ ] Error state for the whole form with a clear message is defined (if needed).
- [ ] Primary and Secondary actions are provided with clear labels and are used following common practices.
- [ ] Buttons with built-in loading indicators are provided (if needed).

:book: **Additional resources:**
- [Primary & Secondary Action Buttons – UX Planet](https://uxplanet.org/primary-secondary-action-buttons-c16df9b36150)

## Responsive design :iphone:
- [ ] Design for **small** and **medium** viewports are provided before or at the same time as the **large** viewport.

:book: **Additional resources:**
- [The 100% correct way to do CSS breakpoints](https://medium.com/free-code-camp/the-100-correct-way-to-do-css-breakpoints-88d6a5ba1862)
- [The State Of Mobile First and Desktop First](https://ishadeed.com/article/the-state-of-mobile-first-and-desktop-first/)
