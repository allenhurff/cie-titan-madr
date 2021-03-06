# ADR 5: Validation

## Context and Problem Statement

*   What libraries (If any) will you use for validation of data?
*   How would you integrate the validation of user input throughout the various properties to ensure data integrity?

## Decision Drivers <!-- optional -->

*   [Back-end validation on AWS Lambda and NodeJS](https://medium.com/a-man-with-no-server/back-end-validation-on-aws-lambda-and-nodejs-ca08a1d07fa0)

## Considered Options

*   [VueJS Form Validation](https://vuejs.org/v2/cookbook/form-validation.html) - Form validation is natively supported by the browser, but sometimes different browsers will handle things in a manner which makes relying on it a bit tricky. Even when validation is supported perfectly, there may be times when custom validations are needed and a more manual, Vue-based solution may be more appropriate. Let’s begin with a simple example.
*   [JavaScript Form Validation](https://www.w3schools.com/js/js_validation.asp) - HTML form validation can be done by JavaScript.

## Decision Outcome

*   [JavaScript Form Validation]
