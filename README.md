# Azimuthal Equidistant Map

Azimuthal Equidistant Map is a single-page browser tool for viewing the world with an azimuthal equidistant projection. You can choose a city preset, rotate the projection, zoom the map, show or hide guide layers, and export the current view as a PNG.

## Features

- City presets for major regions
- Latitude, longitude, heading, and scale controls
- Distance readout from the map center
- Toggleable borders, city names, distance circles, center guide, and graticule
- Visual themes, with Classic selected by default
- Mobile-friendly layout with the map above the control panel and a fit-to-view default scale
- PNG export of the current map view

## Usage

Open `docs/index.html` in a browser, or publish the `docs` directory with GitHub Pages.

Controls:

- Drag the map to move the projection center.
- Hold Shift while dragging to rotate the heading.
- Use the mouse wheel or trackpad scroll to zoom.
- Pinch on mobile devices to zoom in and out.
- Select a preset city to center the map there.
- Edit latitude, longitude, heading, or scale directly when precise values are needed.

## Project Structure

- `docs/index.html`: GitHub Pages entry point.
- `src/index.html`: Source copy kept in sync with the published page.

The app loads D3, TopoJSON, and world map data from public CDNs at runtime, so an internet connection is required when opening the page.

## Publishing Notes

Only source and publishable static files should be tracked. Local system files such as `.DS_Store`, dependency folders such as `node_modules/`, environment files, and logs are ignored by `.gitignore`.
