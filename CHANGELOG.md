# Change Log

All notable changes to the extension will be documented in this file.

The format is based on [Keep a Changelog](https://keepachangelog.com/en/1.0.0/),
and this project adheres to [Semantic Versioning](https://semver.org/spec/v2.0.0.html).

### Version 1.0.22

- Changed activation to `onStartupFinshed`. Thanks [justingrote](https://github.com/maptz/maptz.vscode.extensions.customfolding/pull/115)

### Version 1.0.21

- Updates to package dependencies.

### Version 1.0.20

- Added an experimental feature which adds #regions to the Outline window. Set the `maptz.regionfolder.showRegionsInOutline` setting equal to `true`.

### Version 1.0.19

- Added `collapseDefaultRegionsOnOpen` setting.

### Version 1.0.18

- Updated command names to be consistent with normal pattern for executing commands in VSCode. Thanks to [HenryC-3](https://github.com/HenryC-3)

### Version 1.0.16

- Added support for ['jsonc']. Thanks to [riddlew](https://github.com/riddlew).

### Version 1.0.15

- Added support for [`yuml`](https://yuml.me/).

### Version 1.0.14

- Added support for `powershell`.

### Version 1.0.12

- Added support for `javascriptreact` (used by Adobe Extendscript).

### Version 1.0.11

- Official release from preview branch.

### Version 1.0.11-preview3

- Added support for multiple fold definitions per language. Add secondary fold definitions using the `foldDefinitions` field in your language settings.

```json
{
  "maptz.regionfolder": {
    "[javascript]": {
      "foldEnd": "/* #endregion */",
      "foldEndRegex": "/\\*[\\s]*#endregion",
      "foldStart": "/* #region [NAME] */",
      "foldStartRegex": "^[\\s]*/\\*[\\s]*#region[\\s]*(.*)[\\s]*\\*/[\\s]*$",
      "defaultFoldStartRegex": "^[\\s]*/\\*[\\s]*#region[\\s]*default(.*)[\\s]*\\*/[\\s]*$",
      "foldDefinitions": [
        {
          "foldEndRegex": "\\*+/[\\s]*$",
          "foldStartRegex": "^[\\s]*/\\*\\*+",
          "isFoldedByDefault": true
        }
      ]
    }
  }
}
```

### Version 1.0.11-preview2

- Added support for R.
- Added support for ansible YAML.

### Version 1.0.11-preview1

- Added support for SCSS.
- Added closing of default tags on file opening.
- Added new command: `regionfolder.deleteRegion`.
- Added new command: `regionfolder.removeCurrentRegionTags`.
- Added new command: `regionfolder.wrapWithRegionAndComment`.
- Added new command: `regionfolder.selectCurrentRegion`.
- Added new command: `regionfolder.selectCurrentRegionContents`.

### Version 1.0.9

- Added support for `rust`.

### Version 1.0.8

- Added support for `typescriptreact` [Issue #43](https://github.com/maptz/maptz.vscode.extensions.customfolding/pull/43).
- Added support for `shellscript` [Issue #24](https://github.com/maptz/maptz.vscode.extensions.customfolding/pull/24).

### Version 1.0.7

- Added preliminary support for default fold start using the `defaultFoldStartRegex` setting, and the `regionfolder.collapseDefault` command.

### Version 1.0.5

- Added support for `Java`.

### Version 1.0.4

- Fixed issue that command didn't show up in the command palette. [Issue #17](https://github.com/maptz/maptz.vscode.extensions.customfolding/issues/17)

### Version 1.0.3

- Small bug fixes and documentation updates.

### Version 1.0.2

- Added ability to provide configuration for different languages.
- Added support for `vue` [Issue #13](https://github.com/maptz/maptz.vscode.extensions.customfolding/pull/13)
- Added support for `twig` [Issue #15](https://github.com/maptz/maptz.vscode.extensions.customfolding/pull/15)
- Added support for `php` [Issue #16](https://github.com/maptz/maptz.vscode.extensions.customfolding/pull/16)

### Version 1.0.1

- Added support for `golang` [Issue #14](https://github.com/maptz/maptz.vscode.extensions.customfolding/pull/14)

### Version 1.0.0

- This is the official 1.0 release of the extension.

### Version 0.0.11

- Added support for .fish files. [Issue #9](https://github.com/maptz/maptz.vscode.extensions.customfolding/issues/9)

### Version 0.0.10

- Added support for .dart files. [Issue #8](https://github.com/maptz/maptz.vscode.extensions.customfolding/issues/8)
- Added support for .swift files. [Issue #7](https://github.com/maptz/maptz.vscode.extensions.customfolding/issues/7)

### Version 0.0.9

- Updated NPM dependencies

### Version 0.0.8

- Added support for .ahk files. [Issue #1](https://github.com/maptz/maptz.vscode.extensions.customfolding/issues/1)
- Added support for .lua files [Issue #3](https://github.com/maptz/maptz.vscode.extensions.customfolding/issues/3).
- Added support for .sql files. [Issue #4](https://github.com/maptz/maptz.vscode.extensions.customfolding/issues/4)
