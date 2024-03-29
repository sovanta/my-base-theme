# Base UI5 Theme

This is the UI5 Theme for the Demo Library. You can access the Color Schemes and the Base Styling of UI5 Libraries.

  1. [Git flow](#git-flow)
  2. [Usage](#usage)
  3. [Authors](#authors)

## Git flow
Use always feature Branches for the Development inside the Theme. If you do styling for an Library use the following feature Branch flow:

1. Check if the feature Branch **feature/`{LibraryName}`_`{ControlName}`** (e.g. feature/myControlLibrary_Button) exists. 
 - If so checkout. And merge the corresponding develop Branch inside this feature Branch to be sure all new changes are available.
 - If not create that Branch and make sure to use the correct develop Branch from which you will branch.
2. Make your Development or fix on that Branch.
3. If you've finished your development, than merge that Branch back into the development Branch.

## Usage

To use this Library you have checkout the correct master Branch. 

Your're also able to consume the Theme via NPM. Therefor just run the following command or update your package.json:

```sh
npm install sovanta/my-base-theme.git#master
```

And you have to initialize it in your UI5 Bootstrap.

```sh
<script id="sap-ui-bootstrap"
            src="resources/sap-ui-core.js"
            data-sap-ui-libs="sap.m"
            data-sap-ui-theme="base"
            data-sap-ui-compatVersion="edge"
            data-sap-ui-resourceroots='{"sov.comp.projectName": ""}'>
```

If you only need the Color Scheme than you can simply add following line into your Projects less file, to use all the predefined Mixins:
```sh
@import "{PATH_TO_THEME}/Custom/globals/globals.less";
```

## Authors

* **Deniz Cakici** <deniz.cakici@sovanta.com>
* **Sebastian Mahr** <sebastian.mahr@sovanta.com>
* **Daniel Barthel** <daniel.barthel@sovanta.com>
