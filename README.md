# JSON file structure conventions used by FORM
### V1.0_26092019

## Author's note: Work in Progress, will add further documentation and more robust pattern / key-value checking over time

## How to use the JSON schema to validate your JSON files before requesting
Go to https://www.jsonschemavalidator.net/ and paste the contents of the json schema file (found in the schemas/ directory) to try it out in the browser </br>
### OR
Alternatively, to test it directly in your editor (e.g. vscode) you can use the demo file 'demo.json' in the <b>root</b> directory of this repo. <br/>
Some values were left out on purpose to show the functionality of the JSON schema:
- Try hovering over the highlighted areas (the parts that look like they are complaining), you should see the required keys pop up.
- Not all keys are required, but some there are some exceptions: <i>e.g. the (sub)elements are not required, but if included, their properties must exist.</i>
