

#### Values.js

Install the values.js library and use it to generate a list of colors in the App component.

[Values.js Library](https://github.com/noeldelgado/values.js/blob/master/README.md)

```sh
npm i values.js

```

```js
import Values from 'values.js';
new Values('#f15025').all(10);
```

#### Render Colors

Pass the colors list to the ColorList component.

In the ColorList component, iterate over the list of colors and render each one in a SingleColor component. Fix the key problem by providing a unique id for each color.

In the SingleColor component, display the hex value and weight (percent) of each color, and use inline CSS to set the background color of the component.

#### React-Toastify

Import and set up the react-toastify library.

[React Toastify](https://fkhadra.github.io/react-toastify/introduction)

```sh
npm i react-toastify
```

main.jsx

```js
import 'react-toastify/dist/ReactToastify.css';
```

App.jsx

```js
import { ToastContainer, toast } from 'react-toastify';

toast.success('awesome');
toast.error('error message');

return (
  <main>
    ...............
    <ToastContainer position='top-center' />
  </main>
);
```


```

min-height: calc(100vh - 160px); - This line sets the minimum height of the element. It uses the calc() function to subtract 160 pixels from the viewport height (100vh). The viewport height unit (vh) is relative to the height of the browser window. This means the element will take up at least the full viewport height minus 160 pixels.

display: grid; - This line sets the element's display property to 'grid', enabling the use of the CSS Grid Layout module to arrange its child elements in a grid format.

grid-template-columns: repeat(auto-fit, minmax(223.33px, 1fr)); - This line defines the number of columns and their width in the grid. The repeat() function is used with the auto-fit keyword, which automatically calculates the number of columns based on the container's width and the minimum and maximum column widths specified in minmax(223.33px, 1fr). The minimum width is set to 223.33 pixels, while the maximum width is set to 1 fraction (1fr) of the available space.

grid-template-rows: repeat(auto-fit, minmax(96px, 1fr)); - This line defines the number of rows and their height in the grid, similar to the previous property. The repeat() function is used with the auto-fit keyword, and the minmax() function defines the minimum row height as 96 pixels and the maximum height as 1 fraction (1fr) of the available space.
