# Highball

A Sass cocktail with Bourbon.

Being designed for use with the Rails asset pipeline, Bourbon and Neat are somewhat awkward to integrate with an NPM based workflow. Highball provides a simple foundation that brings these libraries together while avoiding complicated Sass setup in the client app.

# Install

Install the `highball` module and its dependencies into a project context:

```
npm install --save-dev highball
```

# Build

Include `highball/foundation` in a project-specific Sass file:

```
@include "highball/foundation";
```

Ensure that the `node_modules` base directory is linked as an `--include-path` in the Sass build.

For instance, with `node-sass`:

```
node-sass --include-path=node_modules project.scss public/project.css
```
