# VolkerWessels ProjectConfigurator Dto Conventions

This repository serves as a central storage of important information about dto's (data transfer objects) that are used in the VolkerWessels ProjectConfigurator. Schemas can be found here that are used in FORM's backend to check incoming projectconfigurationrequests for validity.

## Patch notes
- Included the option to override a model in a house configuration.
- Removed unneccessary or outdated items (most importantly: elementlisted schema)

## Notes
- The back-end does not currently support facade configuration requests. This will be revisited at a later stage.
- A rotation property can be either a vector: {x, y, z} or a number in degrees
- Elementlisted configurations are no longer supported. Only typeconfiguration-based projectconfigurations can be sent

## How to use the JSON schema to validate your JSON files before requesting
### In your browser:
Go to https://www.jsonschemavalidator.net/ and paste the contents of a json schema file in the left textbox. Now you can test if your json files are valid by writing/pasting them in the right textbox. The red messages below will let you know if there are any incorrect or missing parameters/values.
### OR
### In your (compatible) editor:
Alternatively, to test it directly in your editor (we suggest <b>Visual Studio Code</b>), clone or download this repo to your desired location on your PC. Thereafter, you can use the demo file '<b>demo.json</b>' to write your own json and it will automatically be checked for validity in your editor through suggestions or warnings.<br/>
- Try hovering over the highlighted areas (the parts that look like they are complaining), you should see the required keys pop up.
- Not all keys are required, but there are a few exceptions: <i>e.g. the (sub)elements are not required, but if included, their properties must exist.</i>

## Send requests using Swagger UI:
https://hive.vw.asrr-tech.com/api/v3/hive/swagger-ui.html#/configuration-controller

## Check your configuration on the dashboard:
https://volkerwessels.asrr.nl/dashboard/1
