# 🛌 layout-css

> Easy-to-understand layout classes for css, inspired by Figma's Auto Layout and repeatedly having to figure out common website layouts. Implemented in several popular paradigms.

<br/>

Sleep like a baby and kiss those flexbox & CSS grid nightmares goodbye! Rest well, as you effortlessly create HTML layouts without a worry!

Yes - you can center a div with ease 😌

layout-css makes it a breeze to layout HTML with it's easy-to-understand CSS layout classes implmented in the following paradigms below.

- [@layout-css/tailwindcss-plugin](https://github.com/layout-css/tailwindcss-plugin)

_**🚧 Coming soon**_

- [@layout-css/plain-css](https://github.com/layout-css/plain-css)
- [@layout-css/vanilla-extract](https://github.com/layout-css/vanilla-extract) (CSS in JS/TS)

**Note:** docs will differ for each implemention, continue reading for the key concepts or navigate to your implementation of choice to get started.

## Key Concepts

layout-css builds on the idea of utility-first classes popularised by [Tailwind CSS](https://tailwindcss.com/) and introduces the concept of layout classes. The diference is that utility-first clasess wrap a single concept in css where as the a layout class wraps multiple to achive an intent.

### Sizing Layout Classes

Sizing layout classes describe the desired behavior of the dimensions (width & hieght) of an element regardsless of the parent layout class:

- **fill**: width and/or height in parent
- **hug**: the contents of the child content along the width add/or heigh
- **fixed**: the size of the element along the width and/or height

### Single-Panel Layout Classes

Single-panel layout clasess decribe how the child elements behave in the container bases on the following properties:

#### Single Axis (x or y)

> **💡 TIP** single axis layouts map directly to the [_Auto-Layout_](https://help.figma.com/hc/en-us/articles/5731482952599-Using-auto-layout) features in the popular design tool [![figma-logo](https://github.com/layout-css/.github/assets/1035439/772f3948-9167-477b-97ec-79253a397ec1)](https://figma.com)
> and is the inspiration for this library. For each implementation of layout-css the docs will specify how the class maps to Figma Auto-Layout controls.

- spacing: packed together or spaced apart
- **horizontal-alignment**: of child elements in the parent container<br/>
  (left, center, or right)
- **vertical-alignment**: of child elements in the parent container<br/>
  (top, middle, bottom)
- **axis**: x or y the child elments are layed out along.

#### Grid (x & y)

- **horizontal-alignment**: of child elements within the cells of the grid<br/>
  (left, center, or right)
- **vertical-alignmen**t: of child elements within the cells of the grid<br/>
  (top, middle, bottom)

### 🚧 Responsive-Multi-Panel Layout Classes

_Coming soon_
Responsisve-mulit-panel layout classes describe the behaviours commonly seen on websites across the web and how they behave across the different form factors.

- headers & navigation
- content, columns and side bars
- footers
