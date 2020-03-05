# AngularCarousel

This project was generated with [Angular CLI](https://github.com/angular/angular-cli) version 9.0.1.

## setting up angular carousel project
First install latest version of the angulat cli -> npm install -g@angualr/cli@latest

## create project
ng new project name

## configure carousel package 
install NgbBootstrap library
npm install --save @ng-bootstrap/ng-bootstrap

Also, install bootstrap 
npm install bootstrap

Now, add bootstrap in style.scss file
@import "../node_modules/bootstrap/dist/css/bootstrap.min.css";

Most important, Don't forget to add NgbModule in the main module and import in app.module.ts file 

import { BrowserModule } from '@angular/platform-browser';
import { NgModule } from '@angular/core';
import { NgbModule } from '@ng-bootstrap/ng-bootstrap';
import { AppRoutingModule } from './app-routing.module';
import { AppComponent } from './app.component';

@NgModule({
  declarations: [
    AppComponent
  ],
  imports: [
    BrowserModule,
    AppRoutingModule,
    NgbModule
  ],
  providers: [],
  bootstrap: [AppComponent]
})