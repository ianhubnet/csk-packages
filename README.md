# 🧩 CSK Packages

This repository serves as the **central monorepo** for all **CodeIgniter Skeleton (CSK)** packages — including modules, plugins, themes, libraries, helpers, and language packs.

Each package is managed as a **Git submodule**, enabling independent development, versioning, and distribution — while maintaining a unified structure for automation, updates, and releases.

## 🗂️ Repository Structure

Packages are organized by type:

```
packages/
├──helpers/
├──languages
├──libraries/
├──modules/
├──plugins/
├──themes/
```

Each subfolder contains official CSK components, many of which are private.

| Type      | Description                                  | Access |
| --------- | -------------------------------------------- | :----: |
| Helpers   | Common utility functions                     |   🔒   |
| Languages | Translation packs                            |   🔒   |
| Libraries | Reusable backend logic                       |   🔒   |
| Modules   | Extend core functionality (e.g., Blog, Shop) |   🔒   |
| Plugins   | Add features or integrations                 |   🔒   |
| Themes    | Frontend Themes                              |   🔒   |

## 🛠️ Purpose

* Keep all official CSK extensions organized in one place.
* Provide a base for the CSK **in-app Marketplace**.
* Simplify updates, packaging, and distribution pipelines.
* Serve as a backend dependency hub for production builds.

## Automation
New packages register themselves automatically when:
- They follow the naming convention `csk-<type>-<name>`.
- They define the following repository variables:
  - `CSK_STRIP` → prefix to strip (e.g., `csk-module-`).
  - `CSK_TYPE` → type of the package (`modules`, `themes`, etc.).
  - `CSK_PAT` → personal access token for communication.

> 🪄 This system allows decentralized development while maintaining a synchronized ecosystem.

---

## Example
| Type | Example Repo | CSK_STRIP | CSK_TYPE | CSK_PAT | Added Under |
|------|--------------|-----------|----------|---------|-------------|
| Module | `csk-module-pages` | `csk-module-` | `modules` | `<secret>` | `packages/modules/pages` |
| Theme | `csk-theme-default` | `csk-theme-` | `themes` | `<secret>` | `packages/themes/default` |
| Helper | `csk-helper-array` | `csk-helper-` | `helpers` | `<secret>` | `packages/helpers/array` |

---

> 🚀 CSK uses this monorepo to build update bundles and power its in-app marketplace.


## 🔗 Related Repositories

* [`csk-core`](https://github.com/ianhubnet) — Main CSK Framework *(Private)*
* [`csk-projects`](https://github.com/ianhubnet/csk-projects) — All CSK projects *(Public index)*

---

> This repository is part of the **Ianhub CSK ecosystem**. Most submodules are private, but their structure and organization are visible for transparency and documentation.
