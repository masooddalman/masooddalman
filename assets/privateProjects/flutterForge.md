# FlutterForge

> A CLI tool that generates production-ready Flutter projects with pre-configured architecture, modules, and CI/CD pipelines.

<div align="center">
  <img src="./flutterForgeBanner.png" width="600" alt="flutterforge banner">
</div>

<div align="center">
  <img src="./flutterForge.png" width="600" alt="cli screen shot">
</div>


## What is FlutterForge?

FlutterForge scaffolds Flutter projects with a clean, opinionated architecture out of the box. Instead of spending hours wiring up state management, dependency injection, routing, theming, API layers, and CI/CD pipelines, you run a single command and get a project that's ready for feature development.

It generates projects following **MVVM + Clean Architecture** with **Provider** for state management and **GetIt** for dependency injection. Every generated file follows consistent patterns — base view models, repository interfaces, use case layers, and feature-based folder structure.

Beyond initial scaffolding, FlutterForge manages the project lifecycle. You can add or remove modules after creation, and shared files (`main.dart`, `app.dart`, `locator.dart`) are automatically recomposed to reflect the current module set. The CI/CD wizard generates GitHub Actions workflows with deployment to Firebase App Distribution, Google Play Store, and Apple TestFlight.

### Key Capabilities

- **Interactive wizard** — guided project setup with module selection and organization/package name configuration
- **13 modules** — MVVM, logging, service locator, theming, routing, API client, AI service, localization, startup flow, toast notifications, testing, CI/CD, and flavors/environments
- **Screen generator** — `flutterforge screen <name>` scaffolds a complete MVVM screen with auto-injection into locator and router, optional route parameters, and test generation
- **Module lifecycle** — add and remove modules post-creation with automatic dependency resolution
- **CI/CD generator** — GitHub Actions with per-branch builds, Firebase distribution, Google Play upload, TestFlight deployment, auto-publish with release notes
- **Flavors / Environments** — compile-time environment config via `--dart-define-from-file` with per-environment JSON files and interactive config wizard
- **Run & Build commands** — `flutterforge run` and `flutterforge build` with interactive flavor, device, platform, and build mode selection
- **Multi-platform** — Android and iOS by default, with opt-in support for Web, macOS, Windows, and Linux
- **Clean architecture** — domain/data/feature layers with repositories, use cases, and view models
