# HelloWorld


Please Note this code is based on Angular 4: Beginner to Pro by Mosh https://codewithmosh.com/p/angular-master-class


It is using Angular 16 instead of 4. The basic ideas are the same, but with more type strict limitations in Typescript. eg. I notice in Angular 4 of the tutorial you don't need to worry about type issue in Template, but you will now be in 16.

HttpModule from angular/http cannot be found from the Angular 16, replace it with 

import { HttpClientModule } from '@angular/common/http';

updated 29 Jul 2023

In ng16 map operator is not necessary to rebuild an array from the response, as response from httpClient is already an array

update 28 Jul 2023

Another two differences of Angular 16 are that 
and instead of rxjs/add/operator/catch, ng 16 is using import { catchError } from 'rxjs/operators'; and require using a pipe to call it.
and
instead of Observable.throw in ng4,ng 16 is using **throwError**  
from:
https://stackoverflow.com/questions/45207615/cannot-find-the-angular-common-http-module

This project was generated with [Angular CLI](https://github.com/angular/angular-cli) version 16.1.4.

## Development server

Run `ng serve` for a dev server. Navigate to `http://localhost:4200/`. The application will automatically reload if you change any of the source files.

## Code scaffolding

Run `ng generate component component-name` to generate a new component. You can also use `ng generate directive|pipe|service|class|guard|interface|enum|module`.

## Build

Run `ng build` to build the project. The build artifacts will be stored in the `dist/` directory.

## Running unit tests

Run `ng test` to execute the unit tests via [Karma](https://karma-runner.github.io).

## Running end-to-end tests

Run `ng e2e` to execute the end-to-end tests via a platform of your choice. To use this command, you need to first add a package that implements end-to-end testing capabilities.

## Further help

To get more help on the Angular CLI use `ng help` or go check out the [Angular CLI Overview and Command Reference](https://angular.io/cli) page.
# tsAngularProject
