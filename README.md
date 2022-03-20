# TemplateAngularTailwindDaisyuiFirebase

This project was generated with [Angular CLI](https://github.com/angular/angular-cli) version 13.3.0.

## Status

[![CI Angular Build](https://github.com/YasunoriMATSUOKA/template-angular-tailwind-daisyui-firebase/actions/workflows/ci-angular-build.yml/badge.svg)](https://github.com/YasunoriMATSUOKA/template-angular-tailwind-daisyui-firebase/actions/workflows/ci-angular-build.yml) [![CI Angular Unit Test](https://github.com/YasunoriMATSUOKA/template-angular-tailwind-daisyui-firebase/actions/workflows/ci-angular-unit-test.yml/badge.svg)](https://github.com/YasunoriMATSUOKA/template-angular-tailwind-daisyui-firebase/actions/workflows/ci-angular-unit-test.yml)

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
    - Build
    - Unit Test
      - [Karma](https://karma-runner.github.io/latest/index.html) & [Jasmine](https://jasmine.github.io/) ... default
        - [GitHub Actions](https://angular.jp/guide/testing#configure-project-for-github-actions)
        - [Edit `karma.config.js`](https://angular.jp/guide/testing#chrome%E3%81%A7%E3%81%AEci%E3%83%86%E3%82%B9%E3%83%88%E7%94%A8%E3%81%ABcli%E3%82%92%E8%A8%AD%E5%AE%9A%E3%81%99%E3%82%8B)

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
