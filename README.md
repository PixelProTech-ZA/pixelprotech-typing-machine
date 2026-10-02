# PixelProTech Typing Machine

A free typing-practice app for learners. Seven practice modes (beginner, office, data capture, coding, CV, government forms, speed), timed tests of 15 / 30 / 60 / 120 seconds or untimed, live WPM and accuracy, levels and daily missions.

Made by PixelProTech Solutions (Pty) Ltd. Free to use, provided as is.

## What you need
- Any current Chrome, Edge, Firefox or Safari (a browser from the last few years). No installation, no account, no internet needed once it has loaded.
- A keyboard. It is a typing app; phones work but a real keyboard is the intended use.

## Three ways to deploy (pick one)

**A. Website (easiest to keep updated).** Upload every file in this folder, all in the same folder with no sub-folders, to any web host (for example GitHub Pages). Open the address once on each computer while online. After that it works offline and can be installed from the browser's address bar ("Install app").

**B. School server or intranet.** Copy the folder to any web server in the lab and open its address. The offline and install features need the address to be `https://` or `http://localhost`.

**C. USB stick or local copy (no network at all).** Copy the whole folder to the computer and double-click `index.html`. It runs fully. Offline caching and "Install" are not available this way, and are not needed because the files are already on the machine.

Keep all files together in the one folder. The app needs every file in it (the `.woff2` files are the fonts).

## Where learner data goes
Nothing leaves the computer. There is no account, tracking, analytics or network request. Level, XP, best WPM, top 5 scores and daily missions are saved in the browser on that computer only.

## Shared lab computers
All learners on the same computer and browser profile share one set of progress. Before the next learner, press **RESET MY PROGRESS** (Operator Profile card). It asks for confirmation and clears everything saved by the app. Clearing the browser's site data does the same.

## Updating
Put the new files over the old ones. Open `service-worker.js` and change the `VERSION` text (for example `pixelprotech-typing-v4` to `-v5`) so computers pick up the change. A computer receives it the second time the app is opened while online.

## Troubleshooting
- **Typing does nothing:** click inside the typing area, or press START TEST.
- **Fonts look plain:** a `.woff2` file is missing from the folder. Copy the full folder again.
- **Progress will not save:** the browser is blocking storage (private window, or a locked-down policy). The app shows a "could not be saved" message. Use a normal window.
- **An old version keeps showing:** open the app online twice, or clear the site data for the address.

## Limitations
- Progress is per computer, not per learner, and there is no teacher dashboard or export.
- The scores table shows only that computer's own top 5 results.
- Performance on very old machines has not been tested.
