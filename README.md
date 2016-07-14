# Age Limit Validator Directive - AngularJs

An AngularJs directive that will validate if minimum age requirement is meet based from the entered date on the textbox.

# How to use?

1. Include the library in your existing library AngularJs library like this?
    <pre>
    angular.module('app', ['app.widget'])
             .controller('YourController', ['$scope', function($scope) {                 
             }]);
    </pre>

2. Use the directive on your view like this
    ```html
      <input 
        ng-model="birthday" 
        type="text"       
        age-limit 
        min-age="18"                                          
        under-age-msg="You need to be at least 18 years old."
        title = "Please enter a valid birthdate."                                           
       >
    ```