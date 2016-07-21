# babel-plugin-transform-mjml-import-to-string
MJML imports to strings


```html
<!-- example.mjml -->
<mjml>
  <mj-body>
    <mj-container>
      <mj-section>
        <mj-column>
          <mj-text font-size="40">
            Hello world
          </mj-text>
        </mj-column>
      </mj-section>
    </mj-container>
  </mj-body>
</mjml>
```


```js
// example.js
import mjml from './example.mjml';
console.log(mjml);
// '<mjml>
//   <mj-body>
//     <mj-container>
//       <mj-section>
//         <mj-column>
//           <mj-text font-size="40">
//             Hello world
//           </mj-text>
//         </mj-column>
//       </mj-section>
//     </mj-container>
//   </mj-body>
// </mjml>'
```

## Installation

```sh
$ npm install babel-plugin-transform-mjml-import-to-string
```

## Usage

### Via `.babelrc` (Recommended)

**.babelrc**

```json
{
  "plugins": ["transform-mjml-import-to-string"]
}
```

### Via CLI

```sh
$ babel --plugins transform-mjml-import-to-string index.js
```

### Via Node API

```javascript
require("babel-core").transform("code", {
  plugins: ["transform-mjml-import-to-string"]
});
```
