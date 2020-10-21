---
title: Host your web apps with Azure App Service
author: Speaker Name
---

## What is App Service❓ What are Web Apps❓

### App Service

:::::::::::::: {.columns}
::: {.column width="50%"}

- Really cool
- Even more cool
- Didn't I say it was cool!

:::
::: {.column width="50%"}

![ ][images-app_services]

:::
::::::::::::::

### App Service Web Apps

### Container-based Web Apps

### Code-based Web Apps

Oryx ([github.com/microsoft/oryx][])

## Demo: Deploying an App Service Web App from a container

::: notes

1. Step one

:::

## That's cool, how about the new App Service Static Web Apps❓

### App Service Static Web Apps

### Parts of a Static Web App

- Web application
- Function
- Static content

### Deploying directly from GitHub

GitHub Action ([github.com/azure/static-web-apps-deploy][])

### Example Github Actions workflow YAML

```yml
- uses: Azure/static-web-apps-deploy@v0.0.1-preview
  with:
    azure_static_web_apps_api_token: ${{ secrets.AZURE_STATIC_WEB_APPS_API_TOKEN }}
    repo_token: ${{ secrets.GITHUB_TOKEN }}
    action: "upload"
    app_location: "/"
    api_location: "api"
    app_artifact_location: "public"
```

## Demo: Deploying an App Service Static Web App from code on GitHub

::: notes

1. Step one

:::

## Wrapping up

### Review

- App Service
- Web Apps
  - Container-based
  - Code-based (Oryx)
- Static Web Apps
  - Site content, Function, static content
  - GitHub Actions

### Links

- [github.com/microsoft/oryx][]
- [github.com/azure/static-web-apps-deploy][]

[images-app_services]: media/app_services.png
[github.com/microsoft/oryx]: https://github.com/microsoft/oryx
[github.com/azure/static-web-apps-deploy]: https://github.com/azure/static-web-apps-deploy
