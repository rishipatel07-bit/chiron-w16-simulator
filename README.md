# Bugatti Chiron W16: Interactive Engine

A browser-based 3D simulation of the Bugatti Chiron's 8.0 L quad-turbo W16 engine, built with three.js. No build step and no dependencies to install.

## Live Demo

[Open the interactive engine simulation](https://rishipatel07-bit.github.io/chiron-w16/)

## Features
- A W16 with brushed-metal finish, black head covers, big silver intake pipes, a tight four-turbo cluster and a ribbed seven-speed gearbox, pulled apart in a workshop with a purple car body in the background
- Four-stroke cycle: click a piston to follow one cylinder through intake, compression, power and exhaust, with moving valves, camshaft lobes and colored gas
- Correct crank kinematics: all sixteen rods ride on eight crank pins
- Live telemetry: rpm, power (PS), torque (Nm) and estimated boost (bar)
- Teardown slider lifts the block and heads, drops the sump, raises the intake, and slides the turbo cluster and gearbox away
- Click any part to read about it. Drag to orbit, scroll to zoom
- Motion runs in 1/25 slow motion so the mechanism stays readable

## Run locally
Open `index.html` in a browser (internet needed for three.js and fonts from CDNs).

## Publish with GitHub Pages
1. Create a new repository on GitHub, then in this folder run:
   `git init && git add . && git commit -m "Chiron W16 simulation" && git branch -M main`
   `git remote add origin https://github.com/<you>/<repo>.git && git push -u origin main`
2. In the repository, open Settings, then Pages. Under Build and deployment choose Deploy from a branch, select `main` and `/ (root)`, and save.
3. After a minute your site is live at (https://rishipatel07-bit.github.io/chiron-w16/).

## Docs
See [docs/ENGINEERING.md](docs/ENGINEERING.md) for the engineering model and its limits.

## Credits
Built with three.js (r128). Independent educational project, not affiliated with or endorsed by Bugatti.
