# SERVER SETTINGS

## **Important Note** ---> _READ FIRST!_ <---

This folder contains three files that **MUST NOT** be edited directly!

### **_DO NOT EDIT:_**

- example.env
- settings.development.json
- settings.schema.json

...read below how you should customize/override/provide your own settings instead:

## Provide environment variables: `.env`

The **`.env`** file contains settings that are required for starting the database and oauth2 servers.

A custom `.env` file **MUST** be created in `production` mode.

During `development`, this file is optional, if the `.env` is present the variables in that file will override the development defaults.

Review the `example.env` file for further instructions.

## Provide settings: `settings.json`

A custom **`settings.json`** file must be created when in `production` mode.

During `development` mode, the `settings.json` file is optional. In development mode the settings in the `settings.development.json` will be used. But if a `settings.json` file is present, any settings in that file will override the development defaults.

---

## About the JSON schema file

The **settings.schema.json** file is present for:

- providing autocompletion in your editor,
- validating your JSON settings,
- generating a Typescript type definition file.

---

## @todo

Improve the documentation in this file:

- Add description of JSON settings schema properties
- Add description of environment variables
