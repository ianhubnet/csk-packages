# 🧩 CSK Packages

This repository serves as the **central monorepo** for all **CodeIgniter Skeleton (CSK)** packages — including modules, plugins, themes, libraries, helpers, and language packs.

Each package is managed as a **Git submodule**, enabling independent development, versioning, and distribution — while maintaining a unified structure for automation, updates, and releases.

## 🗂️ Repository Structure

```
packages/helpers/
packages/languages
packages/libraries/
packages/modules/
packages/plugins/
packages/themes/
```

Each subfolder contains official CSK components, many of which are private.

| Type      | Description                                  | Access |
| --------- | -------------------------------------------- | :----: |
| Helpers   | Common utility functions                     |   🔒   |
| Languages | Translation packs (via submodules)           |   🌐   |
| Libraries | Reusable backend logic                       |   🔒   |
| Modules   | Extend core functionality (e.g., Blog, Shop) |   🔒   |
| Plugins   | Add features or integrations                 |   🔒   |
| Themes    | Frontend Themes                              |   🔒   |

## 🛠️ Purpose

* Keep all official CSK extensions organized in one place.
* Provide a base for the CSK **in-app Marketplace**.
* Simplify updates, packaging, and distribution pipelines.
* Serve as a backend dependency hub for production builds.

## 🔗 Related Repositories

* [`csk-core`](https://github.com/ianhubnet) — Main CSK Framework *(Private)*
* [`csk-app-default`](https://github.com/ianhubnet/csk-app-default) — Default boilerplate app *(Public)*
* [`csk-languages`](https://github.com/ianhubnet/csk-languages) — All CSK translations *(Public index)*

---

> This repository is part of the **Ianhub CSK ecosystem**. Most submodules are private, but their structure and organization are visible for transparency and documentation.
