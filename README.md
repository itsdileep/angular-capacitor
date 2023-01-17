# Setup angular app with Capacitor run time

ng new angularCapacitor --routing --style=scss
cd ./angularCapacitor

# Add Capacitor
npm install @capacitor/core
npm install @capacitor/cli --save-dev

# Setup the Capacitor config
npx cap init

npm install @capacitor/ios @capacitor/android
npx cap add ios
npx cap add android

# Build the Angular app
ng build --prod

# Sync the build folder to native projects
npx cap sync

#Open the app with respective Editor and build the app
npx cap open ios
npx cap open android




# AngularCapacitor

This project was generated with [Angular CLI](https://github.com/angular/angular-cli) version 15.1.1.

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
