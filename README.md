# Simple Data Manipulation Language 1 Mentz Challenge

DRAFT CHALLENGE - YOU CAN WORK ON THIS BUT IT MAY CHANGE UNDER YOU
## About
For an overview of Mentz, see the [Blog Post](http://bobbuzzard.blogspot.com/2019/05/introducing-mentz-salesforce-developer.html)
 
This challenge is based on unit testing an Apex trigger that delegates to a utility class method

The following Trailhead modules are available to learn more about unit testing in Apex:

* [Apex Testing](https://trailhead.salesforce.com/en/content/learn/modules/unit-testing-on-the-lightning-platform)
* [Unit Testing on the Lightning Platform](https://trailhead.salesforce.com/en/content/learn/modules/unit-testing-on-the-lightning-platform)


## Taking the Challenge

To take the challenge you build out the ./force-app/main/default/LeadUtils_Test.cls class to cover all scenarios you can identify. Note that 100% test coverage does not indicate all scenarios are covered! Check all of your unit tests pass before submitting your solution. There are a couple of ways of doing this.

### Scratch Org
If you want to iterate on your development, use the Salesforce CLI force:source:push/pull commands to deploy to your scratch org and execute the unit tests.

### Developer Edition
To deploy to a non-scratch org, use:

`sfdx force:source:deploy -p ./force-app/ -u <username>`

if you don't want to deploy the code, you can carry out a check deployment and execute the tests to get the results:

`sfdx force:source:deploy -l RunSpecifiedTests -r LeadUtils_Test -c -u <username> -p ./force-app/`

## Publishing the solution

Ensure you have installed the [MENTZ sfdx plugin](https://www.npmjs.com/package/mentz).

Execute the following command: 

`sfdx mentz:publish -c "<comment>" -f force-app/main/default/classes/LeadUtils_Test.cls -u <username>`

Parameters:

Name | Description
--- | ---
`<comment>` | a comment that raises any areas of concern to the mentor
`<solution_filename>` | the full pathname to your solution class
`<username>`  | your username in the Mentz instance

