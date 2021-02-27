
## Solution of Challenge 2 for Trivago Marketing QA Engineer position



**Task II: Test Automation**

Design a test automation framework for room5.trivago.com that will allow other QA Engineers to  be able to create test cases efficiently. 

**Please cover the following scenarios: **

- Search for any location on Magazine by using the search bar 
- Fill in the contact form and send it (accessible through the footer) 
- Subscribe to the Newsletter 
- Navigate to a destination through the menu on the top left 
- Verify that the links in homepage are working 


**Bonus Scenario (Optional):** 
 
1- Click on Read more button in the Hero Image (hint : class="hero-button" ) 2- Open the browser console 
3- Access the dataLayer of the browser 
4- Check the below events are fired : 
• “OneTrustLoaded” 
• “OptanonLoaded” 
• “OneTrustGroupsUpdated” 

Check every event will include these 4 parameters inside : “C0001,C0003,C0002,C0004" Check “contentLoaded” event is fired then inside the event check the hotelIds is not  empty and the target-properties has the same path in the URL :  
https://magazine.trivago.com/affordable-christmas-vacations-for-families/ 



I have selected Cypress to automate these scenarios because of the cross browser support, CI/CD integration and built-in waiting mechanism making it the ideal choice for web automation. 

I would chose automation in order to perform Regression testing. A good practice is to have two different suites: a very fast regression test that can be executed on every deploy of a development branch, and a more robust regression testing suite that can be executed periodically (like overnight or only before release). 

# Steps to setup Cypress:

```
npm install cypress --save-dev

# If you used npm to install, Cypress has now been installed to your ./node_modules directory, with its binary executable accessible from ./node_modules/.bin.

# Now you can open Cypress from your project root one of the following ways:
# The long way with the full path

./node_modules/.bin/cypress open

```

## Writing the first spec
Follow the below guide to create your first test case to start understanding the basic directory structure and syntax of Cypress from [here](https://docs.cypress.io/guides/getting-started/writing-your-first-test.html#Write-your-first-test)



## Short Steps:
- Clone this Repository and cd to the repository directory
- Run `npx cypress run` command to execute the automated tests
- Once tests are executed successfully, you will see a report automatically generated by Cypress incdicating the Pass/Fail plus the time taken by each test
- Enjoy Testing!

## Long Steps:

- git clone https://github.com/mujjazi/curly-octo-potato.git
- cd .\curly-octo-potato\
- npm init
- npm install cypress --save-dev
- npx cypress open (manual execution)
or
- npx cypress run (automated execution)


### Author
Mujtaba Mehdi,
Feel free to connect on LinkedIn to discuss collaboration ideas.
[LinkedIn](https://www.linkedin.com/in/mujtabamehdi9)
