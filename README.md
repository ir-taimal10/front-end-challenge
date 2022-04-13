# Code Challenge

## How to install the project

This is a mono-repository built with Lerna https://lerna.js.org/

For its execution, the following commands must be run
in the root of the directory where the project was downloaded:

1. `npm i`
2. `npx lerna clean -y`
3. `npx lerna bootstrap --hoist`
4. `npm run start`


In this way, the two projects can be viewed 
__items-api__ runs at http://localhost:5000  
__items-web__ runs at http://localhost:3000


# Packages of the project

## items-api
This application allows to expose 2 endpoints to obtain the items data, the items-api was built using hexagonal architecture to allow to isolate the libraries from the business logic.
![alt text](https://github.com/ir-taimal10/front-end-challenge/blob/master/packages/items-doc/images/hexagonal_arch.PNG?raw=true)


This project is build with Node Js and Express, and makes a REST API available. Ex: http://localhost:5000/rest/items?q=piano
Run with the next lines:
1. `cd packages/items-api`
2. `npm run start`

## items-web
The items-web package was built using React and Redux, Redux makes it possible to manage the states of the application in a simple way.

![alt text](https://github.com/ir-taimal10/front-end-challenge/blob/master/packages/items-doc/images/redux.PNG?raw=true)

The project allows to query ML products using urls like the next:

 * http://localhost:3000/items/MLA1116890684
 * http://localhost:3000/items/MLA1100825910



## Unit tests
unit tests allow to guide the development of each component and to test the different behaviors in each method.
Alister Scott suggests that a testing strategy should be based mostly on automated testing, with more effort on unit testing.

![alt text](https://github.com/ir-taimal10/front-end-challenge/blob/master/packages/items-doc/images/unit_test.PNG?raw=true)


To run the unit tests run:

1. `cd packages/items-web/`
2. `npm run test`

## Behavior test
https://github.com/cucumber/cucumber-js


## Random test
https://github.com/marmelab/gremlins.js
https://marmelab.com/gremlins.js/

## Load test
https://github.com/grafana/k6
