# Tukio Dashboard

## Installation

Install Node.js (recommended latest LTS version). The dashboard uses **Vite** for frontend tooling, to peform installation and building the production version.

Navigate to the project root and run:

```bash
npm install
```

Install Netlify functions:

```bash
npm install --save-dev netlify-cli
npm install @netlify/functions
```

Thats it - to run locally including netlify functions (which is probably what you want):

```bash
netlify dev
```

Or just the frontend:

```bash
npm run dev
```

Confirm its working locally at:

- Dashboard [localhost:5173](http://localhost:5173)
- Functions [localhost:8888/api/hello](http://localhost:8888/api/hello) or [here](http://localhost:8888/.netlify/functions/hello)

## Production Build

Run:

```bash
npm run build
```

This command will generate /dist as build folder. Github will trigger a CI/CD workflow to Netlify at:

- Dashboard [https://tukioii.netlify.app/](https://tukioii.netlify.app/)
- Functions [https://tukioii.netlify.app/api/hello)](https://tukioii.netlify.app/api/hello)

## Template 

For more info refer to [source instructions and install notes](/README.md)