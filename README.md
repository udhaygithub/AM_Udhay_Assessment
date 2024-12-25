# AM_Udhay_Assessment
Technical Assessment

Quick Steps to run the test suite: 

**Step 1.**	Goto https://github.com/udhaygithub/AM_Udhay_Assessment.git and download this file in your machine and unzip it - Playwright_Assessment_AM_1.zip

**Step 2.**	Import this file in your vscode

**Step 3.**	Install playwright dependencies as listed in this section - Pre-Requisites & Dependencies. 
        
        i)	npm install
                      This command should install the below:
                      •	Playwright (@playwright/test)
                      •	Cucumber (@cucumber/cucumber)
                      •	TypeScript support (@types/node, ts-node)
                      •	Utilities like cross-env, dotenv, fs-extra & winston
                      •	Report generation tools (multiple-cucumber-html-reporter)
        ii)	npx playwright install
       iii)	npm install typescript --save-dev
        iv)	npm install ts-node --save-dev (for pre-test & post-test setup)
            
            Note: Also refer package.json file for the dependencies. Screenshot attached in the .doc file

**Step 4.**	For any parallel execution, change the numbers accordingly. (cucumber.js)

**Step 5.**	Use browserManager.ts under helper for cross browsers. Note: Application is working fine on Chrome & Webkit., but not compatible on firefox, just FYI.

**Step 6.**	Use TAGS section if you want to execute a specific Feature file. Currently it is set to run all the files.

**Step 7.**	Use Hooks.ts and change FAILED/PASSED for video, screenshot and error logs. I have currently set it to PASSED, meaning these will appear in the report for a successful test execution

**Step 8.**	Makesure the test is running in headless = !true. Kindly change it under src>helper>browsers> browserManager.ts.
            Currently it is set to headless = true

**Step 9.**	Run the test using terminal – npm run test. Makesure the terminal is pointing to the corresponding folder. Note: dryRun value is currently set to false. Change if needed (cucumber.js)

**Step 10.**	Once the test is executed successfully, Go to test-results folder > reports > index.html to view the full report dashboard

**Step 11.** Kindly also refer screenshots in the word document for further details if required - AM_Assessment_Playwright_ReadMe.doc, attached in this root folder
