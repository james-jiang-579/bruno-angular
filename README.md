# bruno-angular

A starter Angular application scaffolded as a single-project Angular workspace.

## Requirements

- Node.js `^22.22.3`, `^24.15.0`, or `^26.0.0`
- npm

Angular's compatibility table lists these Node.js versions for Angular 22. See [Angular version compatibility](https://angular.dev/reference/versions).

## Getting started

```bash
npm install
npm start
```

Then open <http://localhost:4200/>. To create a production build, run:

```bash
npm run build
```

## Project structure

- `src/main.ts` bootstraps the standalone Angular application.
- `src/app/` contains the root component and its template and styles.
- `angular.json` configures the Angular CLI workspace and build targets.

This workspace uses Angular's standalone APIs and zoneless change detection. It is a minimal starting point; add routes, features, and tests as the application grows.
