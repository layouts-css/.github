# 🛌 layout-css
<div class="info-panel">
    Easy-to-understand layout classes for css, implemented in several popular paradigms.
</div>
<br/>
<style>
    .info-panel {
        font-size: 1.2rem;
        padding: 10px;   
        background-color: #eff6ff;
        border-left: 4px solid #007bff; 
    }
    .tip-panel {
        padding: 10px;   
        background-color: #ecfdf5;
        border-left: 4px solid #34d399; 
    }
</style>



Say goodbye to flexbox or grid headaches and create HTML layouts with ease!

Yes - you can center a div with ease 😌


Layout CSS makes it a breeze to layout you HTML with it's easy-to-understand CSS layout classes implmented in the following paradigms.

- [@layout-css/tailwindcss-plugin](https://github.com/layout-css/tailwindcss-plugin)

_**🚧 Coming soon**_
- [@layout-css/plain-css](https://github.com/layout-css/plain-css) 
- @layout-css/vanilla-extract (CSS in JS/TS)

## Key Concepts

**Layout Classes:** layout-css builds on the idea of utility-first classes popularised by tailwindcss and introduces the concept of layout classes. The diference is that utility-first clasess wrap a single concept in css where as the a layout class wraps multiple to achive an intent.

**Dimension Layout Classes**
Dimension layout classes describe the desired behavior of the dimensions (width & hieght) of an element regardsless of the parent layout class:
- **fill**: width and/or height in parent
- **hug**: the contents of the child content along the width add/or heigh
- **fixed**: the size of the element along the width and/or height

### Single-Panel Layout Classes
Single-panel layout clasess decribe how the child elements behave in the container bases on the following properties:




#### Single Axis (x or y)
<div class="tip-panel">
    
**💡 TIP** single axis layouts map directly to the [_Auto-Layout_](https://help.figma.com/hc/en-us/articles/5731482952599-Using-auto-layout) features in the popular design tool <a href="https://figma.com"><svg xmlns="http://www.w3.org/2000/svg" viewBox="0 -0.10000000000000853 960.6 264.50000000000006" height="12"><path d="M232.2 0v204l26.2.1V107h63.3V81.3h-63.3V25.7h82.4V0zM388.1 41.4c9.5 0 17.1-7.7 17.1-17.1s-7.7-17.1-17.1-17.1c-9.5 0-17.1 7.7-17.1 17.1s7.7 17.1 17.1 17.1zM374.8 67.1V204H401V67.1z"/><path clip-rule="evenodd" d="M498.3 63.1c-34.9 0-59.2 29.5-59.2 64.5s24.3 64.5 59.2 64.5c16 0 29.1-6.2 38.7-16.2V194c0 22.7-17.8 41.6-41.1 41.6-8.4 0-16.7-3.2-23.3-7.8l-13.2 22.8c10.5 6.8 23 10.7 36.4 10.7 37.2 0 67.3-30.1 67.3-67.3V67.1H537v12.2c-9.6-10-22.7-16.2-38.7-16.2zm-32.9 64.5c0-21.7 16.6-38.8 35.8-38.8s35.8 17.1 35.8 38.8-16.6 38.8-35.8 38.8-35.8-17.1-35.8-38.8z" fill-rule="evenodd"/><path d="M657.8 88.8c-15.5 0-28.1 13.2-28.1 28.7V204h-26.2V67.1h26.2v12.5c7.7-9.9 19-16.5 33.8-16.5 18.4 0 32.5 9.1 40.7 23.1 9.1-13.5 23.9-23.1 41.8-23.1 29.9 0 48.5 24.1 48.6 53.9v87h-26.2v-86.6c0-15.5-12.6-28.7-28.1-28.7s-28.1 13.2-28.1 28.7V204H686v-86.6c-.1-15.5-12.7-28.6-28.2-28.6z"/><path clip-rule="evenodd" d="M934.4 82.6c-11.7-12.1-27.7-19.5-46.2-19.5-39 0-66.8 33.1-66.8 72.5s27.7 72.5 66.8 72.5c18.5 0 34.5-7.5 46.2-19.5V204h26.2V67.1h-26.2zm-86.7 53c0-26.1 20-46.8 43.4-46.8 23.3 0 43.4 20.6 43.4 46.8 0 26.1-20 46.8-43.4 46.8-23.4-.1-43.4-20.7-43.4-46.8z" fill-rule="evenodd"/><path d="M0 0h176.3v264.4H0z" fill="none"/><path d="M88.1 132.2c0-24.3 19.7-44.1 44.1-44.1 24.3 0 44.1 19.7 44.1 44.1 0 24.3-19.7 44.1-44.1 44.1-24.3 0-44.1-19.8-44.1-44.1z" fill="#1abcfe"/><path d="M0 220.3c0-24.3 19.7-44.1 44.1-44.1h44.1v44.1c0 24.3-19.7 44.1-44.1 44.1-24.4 0-44.1-19.7-44.1-44.1z" fill="#0acf83"/><path d="M88.1 0v88.1h44.1c24.3 0 44.1-19.7 44.1-44.1 0-24.3-19.7-44.1-44.1-44.1H88.1z" fill="#ff7262"/><path d="M0 44.1c0 24.3 19.7 44.1 44.1 44.1h44.1V0H44.1C19.7 0 0 19.7 0 44.1z" fill="#f24e1e"/><path d="M0 132.2c0 24.3 19.7 44.1 44.1 44.1h44.1V88.1H44.1C19.7 88.1 0 107.9 0 132.2z" fill="#a259ff"/></svg></a> and were the inspiration for this whole library.</div>

- spacing:  packed together or spaced apart
- **x-alignment**: of child elements in the parent container<br/>
(left, center, or right)
- **y-alignment**: of child elements in the parent container<br/>
(top, middle, bottom)
- **axis**: x or y the child elments are layed out along.

#### Grid (x & y)
- **x-alignment**: of child elements within the cells of the grid<br/>
(left, center, or right)
- **y-alignmen**t: of child elements within the cells of the grid<br/>
(top, middle, bottom)


#### 🚧 **Responsive-Multi-Panel Layout Classes:** <br/> [_Coming soon_]
Responsisve-mulit-panel layout classes describe the behaviours commonly seen on websites across the web and how they behave across the different form factors. 
- headers & navigation 
- content, columns and side bars
- footers


