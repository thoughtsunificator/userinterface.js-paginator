# userinterface.js-paginator

Pagination system for userinterface.js

## Getting started

### Installing

- ``git submodule add https://github.com/thoughtsunificator/userinterface.js-paginator.git lib/userinterface.js-paginator``
- ``git submodule update --init --recursive``

### Usage

Binding Prototype: ```function(* application, string model, array entryProps, number entriesPerPage, array entries)```

````html
<!DOCTYPE html>
<html>
<head>
  <script src="./lib/userinterface.js/src/userinterface.js" type="text/javascript"></script>
  <script src="./lib/userinterface.js-paginator/src/object/page.js" type="text/javascript"></script>
  <script src="./lib/userinterface.js-paginator/src/object/paginator.js" type="text/javascript"></script>
  <script src="./lib/userinterface.js-paginator/src/userinterface/page.js" type="text/javascript"></script>
  <script src="./lib/userinterface.js-paginator/src/userinterface/paginator.js" type="text/javascript"></script>
</head>
<body>
<noscript>
  This feature requires JavaScript to be enabled.
</noscript>
<script>
  const application = {}
  const entries = [ "apple", "banana", "orange" ]
  UserInterface.runModel("paginator", {
    parentNode,
    bindingArgs: [application, "yourmodel.entry", [entryProp1, entryProp2], 5, entries]
  })
</script>
</body>
</html>
````

### Live reloading

- ``npm install``
- ``npm start``

### Local

Open index.html.
