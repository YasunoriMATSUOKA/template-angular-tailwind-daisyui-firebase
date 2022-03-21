# TemplateAngularTailwindDaisyuiFirebase

This project was generated with [Angular CLI](https://github.com/angular/angular-cli) version 13.3.0.

## Status

| environment | CI/CD | type               | type       | status                                                                                                                                                                                                                                                                                                         |
| ----------- | ----- | ------------------ | ---------- | -------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| production  | CI    | Angular            | lint       | [![CI Angular Lint](https://github.com/YasunoriMATSUOKA/template-angular-tailwind-daisyui-firebase/actions/workflows/ci-angular-lint.yml/badge.svg)](https://github.com/YasunoriMATSUOKA/template-angular-tailwind-daisyui-firebase/actions/workflows/ci-angular-lint.yml)                                     |
| production  | CI    | Angular            | build      | [![CI Angular Build](https://github.com/YasunoriMATSUOKA/template-angular-tailwind-daisyui-firebase/actions/workflows/ci-angular-build.yml/badge.svg)](https://github.com/YasunoriMATSUOKA/template-angular-tailwind-daisyui-firebase/actions/workflows/ci-angular-build.yml)                                  |
| production  | CI    | Angular            | unit test  | [![CI Angular Unit Test](https://github.com/YasunoriMATSUOKA/template-angular-tailwind-daisyui-firebase/actions/workflows/ci-angular-unit-test.yml/badge.svg)](https://github.com/YasunoriMATSUOKA/template-angular-tailwind-daisyui-firebase/actions/workflows/ci-angular-unit-test.yml)                      |
| production  | CI    | Angular            | e2e test   | [![CI Angular E2E Test](https://github.com/YasunoriMATSUOKA/template-angular-tailwind-daisyui-firebase/actions/workflows/ci-angular-e2e-test.yml/badge.svg)](https://github.com/YasunoriMATSUOKA/template-angular-tailwind-daisyui-firebase/actions/workflows/ci-angular-e2e-test.yml)                         |
| production  | CI    | Firebase Functions | lint       | [![CI Firebase Functions Lint](https://github.com/YasunoriMATSUOKA/template-angular-tailwind-daisyui-firebase/actions/workflows/ci-firebase-functions-lint.yml/badge.svg)](https://github.com/YasunoriMATSUOKA/template-angular-tailwind-daisyui-firebase/actions/workflows/ci-firebase-functions-lint.yml)    |
| production  | CI    | Firebase Functions | build      | [![CI Firebase Functions Build](https://github.com/YasunoriMATSUOKA/template-angular-tailwind-daisyui-firebase/actions/workflows/ci-firebase-functions-build.yml/badge.svg)](https://github.com/YasunoriMATSUOKA/template-angular-tailwind-daisyui-firebase/actions/workflows/ci-firebase-functions-build.yml) |
| production  | CI    | Firebase Functions | unit test  | Not Implemented                                                                                                                                                                                                                                                                                                |
| production  | CD    | Firebase           | deploy all | [![CD Firebase](https://github.com/YasunoriMATSUOKA/template-angular-tailwind-daisyui-firebase/actions/workflows/cd-firebase.yml/badge.svg?branch=v1.0.0&event=release)](https://github.com/YasunoriMATSUOKA/template-angular-tailwind-daisyui-firebase/actions/workflows/cd-firebase.yml)                     |
| development | CI    | Angular            | build      | [![dev CI Angular Build](https://github.com/YasunoriMATSUOKA/template-angular-tailwind-daisyui-firebase/actions/workflows/dev-ci-angular-build.yml/badge.svg)](https://github.com/YasunoriMATSUOKA/template-angular-tailwind-daisyui-firebase/actions/workflows/dev-ci-angular-build.yml)                      |
| development | CI    | Angular            | e2e test   | [![dev CI Angular E2E Test](https://github.com/YasunoriMATSUOKA/template-angular-tailwind-daisyui-firebase/actions/workflows/dev-ci-angular-e2e-test.yml/badge.svg)](https://github.com/YasunoriMATSUOKA/template-angular-tailwind-daisyui-firebase/actions/workflows/dev-ci-angular-e2e-test.yml)             |
| development | CD    | Firebase           | deploy all | [![dev CD Firebase](https://github.com/YasunoriMATSUOKA/template-angular-tailwind-daisyui-firebase/actions/workflows/dev-cd-firebase.yml/badge.svg)](https://github.com/YasunoriMATSUOKA/template-angular-tailwind-daisyui-firebase/actions/workflows/dev-cd-firebase.yml)                                     |

## Links

| environment | URL                                                                                              |
| ----------- | ------------------------------------------------------------------------------------------------ |
| production  | [https://template-angular-firebase.web.app/](https://template-angular-firebase.web.app/)         |
| development | [https://dev-template-angular-firebase.web.app/](https://dev-template-angular-firebase.web.app/) |

## Setup

- [Angular](https://angular.io/guide/setup-local)
  1. `npm install -g @angular/cli`
  1. `ng new template-angular-tailwind-daisyui-firebase`
  1. `cd template-angular-tailwind-daisyui-firebase`
- [Angular ESLint](https://github.com/angular-eslint/angular-eslint)
  1. `ng add @angular-eslint/schematics`
- [eslint-config-prettier](https://github.com/prettier/eslint-config-prettier)
  1. `npm install --save-dev prettier eslint-config-prettier`
  1. Add `"prettier"` in `.eslintrc.json`
- Format on Save Settings
  1. Install ESLint and Prettier as VSCode Extensions
  1. Create `.vscode/settings.json`

```json:settings.json
{
  "editor.defaultFormatter": "esbenp.prettier-vscode",
  "editor.formatOnSave": true
}
```

- [Tailwind CSS](https://tailwindcss.com/docs/guides/angular)
  1. `npm install -D tailwindcss postcss autoprefixer`
  1. `npx tailwindcss init`
  1. Edit `tailwind.config.js`
  1. Edit `src/styles.css`
- [daisyUI](https://daisyui.com/docs/install/)
  1. `npm i daisyui`
  1. Edit `tailwind.config.js`
- CI
  - Angular
    - Lint
    - Build
    - Unit Test
      - [Karma](https://karma-runner.github.io/latest/index.html) & [Jasmine](https://jasmine.github.io/) ... default
        - [GitHub Actions](https://angular.jp/guide/testing#configure-project-for-github-actions)
        - [Edit `karma.config.js`](https://angular.jp/guide/testing#chrome%E3%81%A7%E3%81%AEci%E3%83%86%E3%82%B9%E3%83%88%E7%94%A8%E3%81%ABcli%E3%82%92%E8%A8%AD%E5%AE%9A%E3%81%99%E3%82%8B)
    - E2E Test
      - [Cypress](https://docs.cypress.io/guides/migrating-to-cypress/protractor#Introduction)
  - Firebase
    - Functions
      - Lint
      - Build
      - Unit Test ... Not implemented
- CD
  - Firebase
    - production
    - development
- [Firebase](https://firebase.google.com/)
  1. Create Firebase Projects ... ex. prod: `template-angular-firebase`, dev: `dev-template-angular-firebase`
  1. `npm install firebase`
  1. Set Firebase config in Angular environments
  1. Install CLI tools with `npm i -D firebase-tools` ... `-D` is important!
  1. Execute `npx firebase init` and Initialize default project
  1. Execute `npx firebase use --add` interactively and Set necessary project's alias
  1. Execute `npx firebase init --project=projedt-name` to initialize projects are not default project
  1. Fix functions eslint
  1. Deploy `npx firebase deploy --project=dev-template-angular-firebase --token=${{ secrets.FIREBASE_TOKEN }}` or `npx firebase deploy --project=dev-template-angular-firebase --token=${{ secrets.FIREBASE_TOKEN }}`

## Development server

Run `ng serve` for a dev server. Navigate to `http://localhost:4200/`. The application will automatically reload if you change any of the source files.

## Code scaffolding

Run `ng generate component component-name` to generate a new component. You can also use `ng generate directive|pipe|service|class|guard|interface|enum|module`.

## Build

Run `ng build` to build the project. The build artifacts will be stored in the `dist/` directory.

## Running unit tests

Run `ng test` to execute the unit tests via [Karma](https://karma-runner.github.io).

## Running end-to-end tests

Run `ng e2e` to execute the end-to-end tests via a platform of your choice. To use this command, you need to first add a package that implements end-to-end testing capabilities.

## Further help

To get more help on the Angular CLI use `ng help` or go check out the [Angular CLI Overview and Command Reference](https://angular.io/cli) page.
