# What is it?

Tabby is an open-source window & tab manager that can manage great amounts of windows and tabs at ease.

This is the development branch for Tabby v2.0.

You can install the latest stable version of Tabby on it's Firefox Add-on page: https://addons.mozilla.org/en-US/firefox/addon/tabby-window-tab-manager/<br/>
Or, to install the newest development version, see the [Building, Installing, and Editing](#building-installing-and-editing) section.

# Contributing

If you like this project, please share it. Your support is always welcomed!

Tabby is an open-source project and is in active development, so feel free to submit any issues that you are experiencing and I will do my best to fix it. And if you can fix the issue altogether, feel free to submit a pull request!

My Website: [http://www.WhatsYourIdea.com](http://www.WhatsYourIdea.com)

# Building, Installing, and Editing

## Prerequisites

- Git
- Node.js
- Firefox >= 59 (recommended)<br/>
  or<br/>
  Chrome >= 49 (fully tested on Chrome 72)

## Building Tabby

1. Open a git enabled shell of your choice (e.g. Command Prompt, Git Bash)
2. Get the source code  
`git clone https://github.com/Bill13579/tabby.git`
3. Go into the Tabby directory  
`cd tabby`
4. Switch to the `v2.0-dev` branch  
`git checkout v2.0-dev`
5. Install dependencies with npm  
`npm install`
6. Build Tabby  
Firefox: `npm run build:firefox`  
Chrome: `npm run build:chrome`  
WebExtension: `npm run build:webext`

## Installation

### Firefox
This will install Tabby as a temporary add-on, so you will need to re-do this everytime you restart Firefox.

1. Start Firefox
2. Go to `about:debugging`
3. Press on the `Load Temporary Add-on...` button
4. Select the `manifest.json` file in the `dist` directory

### Chrome

1. Start Chrome
2. Go to `chrome://extensions`
3. Press on the `Load unpacked` button
4. Select the `dist` directory

## Editing & Testing

After you edit the code, you will need to build again.

Re-do Step 6 of [Building Tabby](#building-tabby) and<br/>
- on Firefox, press the `Reload` button in the Tabby section of the `about:debugging` page.<br/>
- on Chrome, press the ![Chrome Reload Icon](data:image/png;base64,iVBORw0KGgoAAAANSUhEUgAAABQAAAAUCAYAAACNiR0NAAABeUlEQVQ4T73Uv0vVURjH8ddVSF01fwxC/lilUEQFoyFoSZFscEukQQ1HRwd1aotCRPwDImwQZ5cgokSHftCU4GLiINQSiRAYj5wrern3K1wuPsv3C+c87/M85/l8Tk6FI1dhnmsDxkHNGMBdNKROfmMH73GIDtzEVr7TYhXeQDdG0It6/MMJYu0PPuMb2lGHuSxgD6bRhy/4iCMcown9GEQ1avEdo6WA0VrAYsMHLGO3YHD3sIj4VmEjCziMGfzC83T6RV4rJjGOW2khEziPgL7BiyKSeoonaLuwtompUi2v4A5eYa0cjRZOOQ98ibeVAC5gCK8R0KwYwyN8wlKplq8aSj4v9DeL24iu4s7PorDlcMczPMQ7rGKvoMxOTOBBqi6Gt58l7LBbQLtSQgg7LBeHh7DDPbHnR6ou9HqaBaxJLnmcLBhuCNuFiOP/L75iPYk/bHkepV6bSG5JbriPxpTxE9vpcThIHr90I9f2fJUjwaJTLhuUT/wPlkdEFU4UYzoAAAAASUVORK5CYII=) button in the Tabby section of the `chrome://extensions` page.

Note: Content Scripts will only be reloaded for each tab once that tab is refreshed.

# File Structure

icons/ - Directory for storing Tabby icons<br/>
icons/tabby.svg - Tabby icon (Vector)<br/>
icons/tabby.png - Tabby icon (Raster)<br/>

release/ - Release zip files<br/>

screenshots/ - Screenshots<br/>
screenshots-archive/ - Old screenshots of old releases<br/>

dist/ - Distribution directory<br/>
src/ - Source code directory (for more info, go to the [README.md](src/README.md) file in that directory)<br/>

LICENSE - License file<br/>
README&#46;md - README file
