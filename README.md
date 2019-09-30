# JSON file structure conventions used by FORM
### V1.0_26092019

## Author's note: Work in Progress, will add further documentation and more robust pattern / key-value checking over time

## How to use the JSON schema to validate your JSON files before requesting
### In your browser:
Go to https://www.jsonschemavalidator.net/ and paste the contents of a json schema file (<b>'vw-project-configurator-schema-project.json'</b> in the /schemas/ directory) in the left textbox. Now you can test if your json files are valid by writing/pasting them in the right textbox. The red messages below will let you know if there are any incorrect or missing parameters/values.</br>
### OR
### In your (compatible) editor:
Alternatively, to test it directly in your editor (we suggest <b>visual studio code</b>), clone or download this repo to your desired location on your PC. Thereafter, you can use the demo file 'demo.json' to write your own json and it will automatically be checked for validity in your editor through suggestions or warnings.<br/>
Some values were left out on purpose to show the functionality of the JSON schema:
- Try hovering over the highlighted areas (the parts that look like they are complaining), you should see the required keys pop up.
- Not all keys are required, but there are a few exceptions: <i>e.g. the (sub)elements are not required, but if included, their properties must exist.</i>

## Send requests using Swagger UI:
http://hive.vw.asrr-tech.com:10000/swagger-ui.html#/configuration-controller
