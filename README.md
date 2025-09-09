# Date Divider

A simple, persistent date divider for your browser tabs.

## Functionality

This page displays a single, large date. It's designed for people who keep many tabs open and want a visual separator to indicate when they opened a set of tabs.

The date displayed is determined by the `date` parameter in the URL.

-   If you visit the page without a date parameter, it will automatically set the parameter to the current date.
-   If you open a link that already has a date parameter, it will display that specific date.

This allows the date to remain fixed when sharing tabs or re-opening them on different devices.

## Usage

1.  **Open the page:** Navigate to the deployed URL. The current date will be displayed and "pinned" in the URL.
2.  **New Divider:** To create a new divider with the current date, simply open the base URL again in a new tab.
3.  **Sharing:** Share the URL from a tab to preserve its pinned date.

## Deployment

This project is a static Astro site and can be deployed to any static hosting provider. It is currently configured for deployment to GitHub Pages.

The deployment is handled automatically by the GitHub Action workflow in `.github/workflows/deploy.yml`. To deploy, simply push your changes to the `main` branch.

## Development Commands

All commands are run from the root of the project, from a terminal:

| Command           | Action                                     |
| :---------------- | :----------------------------------------- |
| `npm install`     | Installs dependencies                      |
| `npm run dev`     | Starts local dev server at `localhost:4321`|
| `npm run build`   | Build your production site to `./dist/`    |
| `npm run preview` | Preview your build locally, before deploying |
