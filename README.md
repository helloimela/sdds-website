# Scania Digital Design System - Website

Visit SDDS at [digitaldesign.scania.com](https://digitaldesign.scania.com/)
## How to get started with @scania/components and @scania/theme-light

For more information how to contribute [Contribution](https://github.com/scania-digital-design-system/sdds/blob/master/CONTRIBUTING.md)

How to report a issue or feature request please visit [digitaldesign.scania.com/contribution](https://digitaldesign.scania.com/contribution)

## SDDS Website
To run this project locally you will need **NodeJS** and **Npm** installed

Clone this repo, install all dependencies and start the application:
```bash
> git clone https://github.com/scania/sdds-website.git
> cd sdds-website
> npm i
> npm start
```

## Locally setup

Run locally with **Angular**
```bash
> cd sdds-website
> npm i
> npm start
```

Visit http://localhost:1337/

## Fetch latest data from SDDS-CMS

To have access to latest data from our headless cms you need to fetch it with follow command:

```bash
> cd sdds-website
> npm run data
```

## Running [@scania/components](https://www.npmjs.com/package/@scania/components) and [@scania/theme-light](https://www.npmjs.com/package/@scania/theme-light) on sdds-website

This is used to be able to run the local version on your computer toghether with the website. To find out more about the SDDS component and themes packages please visit [scania-digital-design-system/sdds](https://github.com/scania-digital-design-system/sdds)


Clone SDDS components and theme from [scania-digital-design-system/sdds](https://github.com/scania-digital-design-system/sdds)

Create npm links of **SDDS components and theme**

```bash
> cd sdds/components
> npm link
> cd sdds/theme/light
> npm link
```

Use npm link to **@scania/components** and **@scania/theme-light** in sdds-website to run everything locally
```bash
> npm run link
  // or
> cd sdds-website
> npm link @scania/components
> npm link @scania/theme-light
```

## Technical notes

It is rendered as follow:
- Content: **src/app/data/content.json** served by **app service**
- Templates: **src/app/data/templates.json** rendered by **page component**
- Router: **Angular router** initiated by **main component**.
