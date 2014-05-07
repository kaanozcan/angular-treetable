### Angular Tree Table  
  
This is a simple Tree Table for Angularjs  
  
Basicly append an element with tree, records and model attributes. tree attribute can be blank, records attribute will point out to the record list on your scope, and model attribute will point out to your model.  
  
model attribute syntax:  
$scope.model = {  
  
  propertyName: 'Label'
};  
  
records syntax:  
$scope.records = [  
  
  property: 'value'  
  children: []
]  
  
html  

<div tree model="model" records="records"></div>
