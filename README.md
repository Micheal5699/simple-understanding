# simple-understanding
           How To Understand Easily
Most people find it so difficult to understand.
To understand is easy as you understand A,B,C
or What you know how to do best.
 Try learning natural visualization, which is 
anything you can create, make use of and that 
brings positive outcome that you can
use, and also the society. After the 
society have made use of it and came out good,
with damage free and has surely provided income
for you and the society. Now you have a big 
priority of what you can easily do.

Selenium Data Drive framework with Maven
https://github.com/netowsolutionsltd/I-Invest-Automation.git

HOW TO GET A RESPONSE BODY FROM INTEGER
var get = JSON.parse(responseBody);
pm.collectionVariables.set("token", get.data[0].beneficiaryId);


SCRIPT TO AUTOMATE A PAGE THAT THE SELECTORS ARE CHANGING
import {Login} from "../fixtures/selectors.js";
Cypress.on('uncaught:exception', (err, runnable) => {
  return false
})

// const access = require("./validLogin.cy.js");
describe("Given I am on the login page", function () {
    beforeEach(function () {
        cy.visit('/')


    });
    it("LOGIN - Invalid Login", function () {
      cy.wait(3000)
      cy.get(Login.emailField).then((element)=>{
        cy.wrap(element).type('Test@yopmail.com');
      })
      cy.get(Login.passwordField).then((element)=>{
        cy.wrap(element).type('TestPassword');
      })
      cy.get(Login.signInBtn).click()
      cy.wait(4000)
      cy.contains('Sign into your account').should("be.visible")

    });
    it("LOGIN - Valid Login", function () {
      cy.wait(3000)
      cy.get(Login.emailField).then((element)=>{
        cy.wrap(element).type(Login.emailText);
      })
      cy.get(Login.passwordField).then((element)=>{
        cy.wrap(element).type(Login.passwordText);
      })
      cy.get(Login.signInBtn).click()
      cy.wait(4000)
      cy.contains('Account').should("be.visible")
    })
})

Link on how to generate a selector

https://www.youtube.com/watch?v=cSa4VAHawMg&t=629s

