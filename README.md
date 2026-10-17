# Multi-Step Form Wizard

A standalone, responsive three-step form demo. It guides the user through personal information, address details, and a final review before showing a completion screen.

## Features

- Three-step progress indicator with current and completed states
- Step-level validation for required fields, email, phone number, and postal code
- Back navigation and edit links that preserve entered values
- Review summary before the final submit action
- Responsive desktop and mobile layout
- No data is transmitted or stored; submission is a front-end demo confirmation

## Run locally

Requires Node.js 20 or newer.

```powershell
npm.cmd ci
npm.cmd run dev
```

## Build

```powershell
npm.cmd run build
```

## Deploy to Firebase Hosting

This standalone app is configured to use a separate Hosting site named `multi-step-form-wizard` in the existing Firebase project. This keeps its deployment separate from Product Search.

Create the Hosting site once if it does not exist yet, then build and deploy:

```powershell
firebase.cmd hosting:sites:create multi-step-form-wizard --project product-search-app-929a5
npm.cmd run build
firebase.cmd deploy --only hosting --project product-search-app-929a5
```

The expected public URL is `https://multi-step-form-wizard.web.app`.
