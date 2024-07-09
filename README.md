# OlympicGamesStarter
<img src="https://github.com/magicfinger96/Developpez-le-front-end-en-utilisant-Angular/assets/23461686/79703304-c38c-4561-9707-033ba20ae3e4" width="500">
<img src="https://github.com/magicfinger96/Developpez-le-front-end-en-utilisant-Angular/assets/23461686/e7ae3dcb-507c-4273-ba8e-0bd16ccc22c4" width="500">

## Context
The TV channel TéléSport would like to create a new web application to prepare the coming Olympic Games.

The goal of this application is to provide, for the users, a dashboard allowing to visualize data about the previous Olympic Games.

## Requirements
- This project is using [Angular CLI](https://github.com/angular/angular-cli) version 18.0.5.
- Don't forget to install your node_modules before starting (`npm install`).

## Development server

Run `ng serve` for a dev server. Navigate to `http://localhost:4200/`. The application will automatically reload if you change any of the source files.

## Build

Run `ng build` to build the project. The build artifacts will be stored in the `dist/` directory.

## Architecture

The architecture includes (in addition to the default angular architecture) the following:
- `components`:
  - `header` folder: handles the page header: title (and back button).
  - `stats-labels-bar` folder: handles the bar of statistics labels
- `pages` folder: contains components used for routing.
  - `detail` folder: contains the component of the Detail page.
  - `home` folder: contains the component of the Home page.
  - `not-found` folder: contains the component of the Not Found Page. (Displayed when the url leads nowhere.)
- `core` folder: contains the business logic:
  - `services` folder:
    - `olympic.service.ts`: handles the olympics logic.
  - `models` folder:
    - `LineChartData.ts` and `LineChartSerieData.ts`: used to fill the line chart in the Detail Page.
    - `OlympicParticipant.ts`: represents a country that has participated to Olympic Games.
    - `Participation.ts`: represents the participation of a country to the Olympic Games.
    - `PieChartData.ts`: used to fill the pie chart in the Home Page.
    - `StatsLabel.ts`: represents statistics label data.
    - `HomePageData.ts`: represents home page data.
    - `DetailPageData.ts`: represents detail page data.
