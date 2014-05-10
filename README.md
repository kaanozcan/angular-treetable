### Angular Tree Table  
  
This is a simple Tree Table for Angularjs which displays and filters both  parent and children objects, dynamically creating fields and filters using the object model passed to it.  
  
Basicly append an element with tree, records and model attributes. tree attribute can be blank, records attribute will point out to the record list on your scope, and model attribute will point out to your model.  
  
Bootstrap needed for + button and input elements you can change the button completely and remove classes from inputs
  
model attribute syntax:  

```
$scope.model = {
  propertyName: 'Label'
};
```
  
records syntax:

```
$scope.records = [{
  property: 'value',  
  children: []  
}]
```

  
html

```
<div tree model="model" records="records"></div>
```
  
Road Map

inline edit
form templates
custom cells rows
  
  
Example

```
$scope.myModel = {
  name: 'Name',
  type: 'Type Name',
  crDate: 'Creation Date'
};

$scope.myRecords = [{
  name: 'Files',
  type: 'Folder',
  crDate: '10.10.2014',
  children: [{
    name: 'Uncle',
    type: 'Image',
    crDate: '11.10.2014',
    children: []
  }, {
    name: 'Sister',
    type: 'Image',
    crDate: '11.10.2014',
    children: []
  }, {
    name: 'Brother',
    type: 'Image',
    crDate: '11.10.2014',
    children: []
  }, {
    name: '12.10.2014 trip',
    type: 'Folder',
    crDate: '12.10.2014'
    children: [{
      name: '12.10.2014_trip78m',
      type: 'Video',
      crDate: '12.10.2014',
      children: []
    }]
  }]
}];

<div tree model="myModel" records="myRecords"></div>

```
