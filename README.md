# Overview

Take look at id.js and figure out what's wrong with it.

The suggested fixes are detailed here in this README below, not inline in the code.

## Essential Code Fixes

1. Add a test for the code: test/id_spec.js (currently does nothing except show any syntax errors or issues like next on this list)
2. Line 8 typeof check must before null check.
3. Line 9 NAMESPACE missing var keyword which puts NAMESPACE in the global context.

## Best practice Code Fixes

1. Line 1 Add 'use strict' statement
2. Line 20 Unused _closed variable

## Code Review Comments

The code as it is appears as plain ES5 Javascript.
A quick improvement would be to use the Revealing Module Pattern which will separate the Public and Private functions.

Further down the best practise and framework path a system like AngularJS, React or Ember should be employed.
