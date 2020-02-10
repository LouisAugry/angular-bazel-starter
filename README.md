# Angular Bazel starter

This project was generated with [Angular CLI](https://github.com/angular/angular-cli) version 9.0.1.

This is a simple starter for Angular with Bazel

## Installation
You only need NodeJS and npm (or yarn).

Install dependencies :

```bash
$ npm i
# or
$ yarn
```

## Development

Run this for a dev server :

```bash
$ ng serve
# or
$ ibazel run //src:devserver
```

This runs in "watch mode", which means it will watch any files that are inputs to the devserver, and when they change it will ask Bazel to re-build them.
When the re-build is finished, it will trigger a LiveReload in the browser.

This command prints a URL on the terminal. Open that page to see the demo app running. As soon as you save a change, the app should refresh in the browser with the new content. Our intent is that this time is less than two seconds, even for a large application.

Control-C twice to kill the devserver.

## Testing

Run all the unit tests:

```bash
$ ng test
# or
$ bazel test //src/...
```

Or run the end-to-end tests:

```bash
$ ng e2e
# or
$ bazel test //e2e/...
```
## Production

We can run the application in production mode, where the code has been bundled and optimized. This can be slower than the development mode, because any change requires re-optimizing the app.

```bash
$ ng serve --prod
# or
$ bazel run //src:prodserver
```
