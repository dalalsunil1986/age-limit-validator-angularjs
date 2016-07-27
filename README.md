# Age Limit Validator Directive - AngularJs

An AngularJs directive that will validate if the set minimum age requirement is meet based from the entered date on the input text box. Directive is using 
HTML5 native form validation so it plays nice on existing HTML5 forms. 


# How to use?

1. Include the library in your existing AngularJs project like this:
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
    
    Use HTML5 form's pattern attribute for accepted date format yyyy-mm-dd ...

    ```html
      <input 
        ng-model="birthday" 
        type="text"       
        age-limit 
        min-age="18"                                          
        under-age-msg="You need to be at least 18 years old."
        pattern="^\d{4}-\d{1,2}-\d{1,2}$"
        title = "Please enter a valid birthdate."                                           
       >
    ```