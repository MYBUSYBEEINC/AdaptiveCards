# React.js Adaptive Cards component

## Install and import the module

### Node

```console
npm install react adaptivecards-react --save
```

```js
// Import the module:
import * as AdaptiveCard from "adaptivecards-react";

// OR require it:
var AdaptiveCard = require("adaptivecards-react");
```

```tsx
import { AdaptiveCard } from "adaptivecards-react";
```

### Usage

Basic usage:

```js
  var card = {
    "type": "AdaptiveCard",
    "version": "1.0",
    "body": [
        {
            "type": "TextBlock",
            "text": "Here is a ninja cat"
        },
        {
            "type": "Image",
            "url": "http://adaptivecards.io/content/cats/1.png"
        }
    ]
  };
<AdaptiveCard
    payload={card}
/>
```

Non-interactible:

```js
<AdaptiveCardView
    payload={card}
    style={{ pointerEvents: 'none' }}
/>
```