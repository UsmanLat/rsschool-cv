# Usman Latipov #


## Contacts ##

**Phone:** +​998972786875
**Email:** LatipovUf@gmal.com


## About me ##
 
Software engineer, with adequate professional experience. 
Worked with a variety of technologies or programming languages. 
An early adopter of new frameworks and libraries. I follow best 
practices and methodologies and constantly use programming 
patterns to build effective systems and applications. Have good 
analytic abilities and work with legacy code. 

## KEY SKILLS ##


 **Front End**
* HTML5, CSS3 
* Javascript
* ReactJS 
* Babel

 
**Back End**
* MySQL
* NodeJS
* PHP
 
**DevOps** 
* Github 

## WORK HISTORY ##

 
**Software Engineer**  
01/2017 – Present 
UHT Software Development  Tashkent, UZ  
* Developed new features for ASP.NET based Applications 
* Web application maintenance and bug fixing 

**Junior Frontend Developer**
07/2015 – 12/2017 
SIS Development  Tashkent, UZ  
* Supported existing and developed new internal services
* Developed a cross-browser adaptive layout
* Participated in the development of the frontend part of the applications.


## SAMPLE CODE ##


...


    (function (window) {
      'use strict';

      let App = window.App || {};
      let $ = window.jQuery;

      function FormHandler(selector) {
        if (!selector) {
          throw new Error('No selector provided');
        }

        this.$formElement = $(selector);
        if (this.$formElement.length === 0) {
          throw new Error('Could not find element with selector: ' + selector);
        }
      }

      FormHandler.prototype.addSubmitHandler = function (fn) {
        console.log('Setting submit handler for form');
        this.$formElement.on('submit', function (event) {
          event.preventDefault();

          var data = {};
          $(this).serializeArray().forEach((item) => {
            data[item.name] = item.value;
            console.log(item.name + ' is ' + item.value);
          });
          //console.log(data);
          fn(data);
          this.reset();
          this.elements[0].focus();
        });
      };

      FormHandler.prototype.addInputHandler = function (fn) {
        console.log('Setting input handler for form');

        this.$formElement.on('input', '[name="emailAddress"]', event => {
          let emailAddress = event.target.value;
          //console.log(emailAddress);
          let message;
          if (fn(emailAddress)) {
            event.target.setCustomValidity('');
          } else {
            message = emailAddress + ' is not an authorized email address!';
            event.target.setCustomValidity(message);
          }
        });
      };

      App.FormHandler = FormHandler;
      window.App = App;
    })(window);

...

## EDUCATION ##

 
**Bachelor degree.** Applied Mathematics and Computer Science, 2011-2015. Uzbekistan National University, Tashkent. 


## LEVEL OF ENGLISH PROFICIENCY ##

CEFR: A2

