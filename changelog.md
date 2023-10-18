## 1.0.0 (2023.10.18)

### Maintenance

- **project**: sets up 1.0.0 release and commitizen

## 0.1.2 (2023-10-17)

### Bug Fixes

- **remote**: removes more window.alerts

## 0.1.1 (2023-10-17)

### Bug Fixes

- **remote**: hard-refreshes the page on test error rather than window.alert

## 0.1.0 (2023-09-21)

### Features

- **report**: adds test index to report output (#30)
- **report**: clears localStorage when clearing input

### Bug Fixes

- **remote**: passes all of `process.env` as part of `env` arg to `child_process.exec`
- **remote**: passes all of `process.env` to include caller env vars
- **remote**: allows subdirectories to also be served at root

### Maintenance

- **project**: bump to version `0.1.0` (#31)

### CI/CD

- **project**: bumps package version in prepareation for release/0.0.4

## 0.0.3 (2023-08-08)

### Features

- **remote**: serves the report and fowards requests for configured bitmaps paths
- **project**: bump version to 0.0.3 for forkedfeatures
- **report**: adds styles/theme to `LogModal`
- **playwright**: adds logging, implements `logger` in playwright runner

### CI/CD

- **playwright**: moves logger declaration

## 0.0.2 (2023-08-06)

### Features

- **compare**: adds `localStorage` filter on reload, server ping before loading ref/test buttons
- **compare**: adds test label link to filter by name; escape key and button clear for filter
- **compare**: adds and applies dark/light theme css variables

### Bug Fixes

- **remote**: adds `--colors` flag to `remote` so `chalk` works in child process

### CI/CD

- **compare**: adds disabled state and alert when backstop remote fails
- **project**: updates playwright and puppeteer to latest

## 0.0.1 (2023-08-05)

### Features

- **project**: upgrades babel and reconfigures webpack
- **remote/report**: adds reference endpoint, button, and filter capability
- **report**: adds favicon etc
- **report**: adds test button, animates button while testing, then reloads upon completion
- **remote**: use report paths from config (#1172)
- **build**: Upgrade to puppeteer@7.1.0 (#1284)
- **loadCookies**: check for http and https in cookie domain (#1264)
- **compare**: exit 1 on fail

### Bug Fixes

- **report**: adds extension back to extraButtons.js
- **report**: fixes button classnames/styles
- **report**: move button state; remove console.log
- **report**: removes openReport customization - handled by config in downstream backstop.config.js
- **report**: adds resolve back to promise
- **remote**: allows the `ApproveButton` component to get its port number from the browser (#1489)
- **remote**: updates `child_process.exec` to include PATH and log errors (#1488)
- **docs**: onBefore / onReady arguments (#1205)
- **report**: #1166 approve button does not work on the filtered failed page. (#1175)
- **report**: disable the button when it is pending. (#1152)
- **readme**: spelling
- **spawn**: add win syntax case

### Refactor

- **compare**: refactors the use of `VisibilitySensor`
- **project**: nukes `backstop.json` and replaces with `backstop.config.js`
- replaced resolve dependency via require.resolve() (#1316)
- replaced resolve dependency via require.resolve() (#1316)
- **waitFor**: replaced .waitFor by its successor .waitForTimeout (#1277)
- **cli**: do not process.exit() + fix cli test (#1125)

### Maintenance

- update playwright from 1.17.1 to 1.20.0 (#1404)
- update puppeteer from 12.0.1 to 13.5.1 (#1403)

### Documentation

- fix typo (#1056)
- **readme**: update approve filter docs to file name (#945)
- **readme**: add contributing section to table of contents (#838)
- **readme**: add windows instructions (#828)
- Update references to configPath (#429)

### CI/CD

- **compare**: inlines ui image assets; adds reports to `.eslintignore`
- **compare**: adds post-upgrade compare build
- **project**: upgrades to a custom backstop-twentytwenty build
- **project**: bumps version number
- **report**: adds button/styles to run tests
- **report**: disables opening report in browser
