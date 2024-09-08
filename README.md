# Cypress Automation Framework

- [Cypress Automation Framework](#cypress-automation-framework)
  - [Initate Cypress Install](#initate-cypress-install)
  - [Open Cypress](#open-cypress)
  - [Recommended Extensions for VS Code](#recommended-extensions-for-vs-code)
  - [Recommended Configuration for VS Code](#recommended-configuration-for-vs-code)
  - [Install Cucumber](#install-cucumber)
    - [Resolve Missing Dependencies](#resolve-missing-dependencies)

## Initate Cypress Install

- Initate package.json

`npm init`

- Install Cypress

`npm install cypress --save-dev`

## Open Cypress

- Add a Script in package.json

`"cypress-open": "cypress open"`

## Recommended Extensions for VS Code

- Markdown All in One
- Material Icon Theme
- Prettier - Code Formatter
- Cucumber (Gherkin) Full Support

## Recommended Configuration for VS Code

```
   "cucumberautocomplete.customParameters": [],
    "cucumberautocomplete.strictGherkinCompletion": true,
    "cucumberautocomplete.steps": [
        "cypress/support/step_definitions/*.js"
    ]
```
- package.json
```
  "cypress-cucumber-preprocessor": {
    "stepDefinitions": "cypress/support/step_definitions/**/*.js"
  }
```
- https://github.com/glennraya/vscode-settings-json (Complete VS Code Customization)


## Install Cucumber

- Install @badeball/cypress-cucumber-processor
`npm install @badeball/cypress-cucumber-preprocessor --save-dev`

Links:
- [NPM](https://www.npmjs.com/package/@badeball/cypress-cucumber-preprocessor)
- [GitHub](https://github.com/badeball/cypress-cucumber-preprocessor)
- Follow the Quick Start Settings and Code
- [FAQs](https://github.com/badeball/cypress-cucumber-preprocessor/blob/master/docs/faq.md)

### Resolve Missing Dependencies

- `npm install @bahmutov/cypress-esbuild-preprocessor --save-dev`
- `npm install ts-loader --save-dev`
