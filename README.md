<h1>Attempt of simple component manager</h1>

- [Key folders](#key-folders)
- [Basic component definition](#basic-component-definition)
  - [Example](#example)
- [How to add components to my html](#how-to-add-components-to-my-html)
- [Quickstart template](#quickstart-template)


## Key folders
---
- components

## Basic component definition
---
### Example
We are going to create an `html` file in the components directory called **navbar.html**
```html
<style>
    div{
        background-color: rgb(72, 115, 233);
        padding: 10px;
        font-weight: bold;
        color: white;
    }
</style>
<div>
    NAVBAR COMPONENT
</div>
```

## How to add components to my html 
---
```html
<!DOCTYPE html>
<head>
    <script src="componentManager.js"></script>
    <title>Test</title>
</head>
<body>
    <div id="navbar"></div>
</body>
</html>
```
Simply add the script `componentManager.js` to your html file, then create or modify a json file called `components.json` in your project root like so:

```json
{
    "components":[
        "navbar"
    ]
}
```

## Quickstart template
You cand find a project template [here](./quickstart-template/)