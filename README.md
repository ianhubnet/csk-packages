# 🧩 CSK Packages

This repository serves as the **central monorepo** for all **CiSkeleton (CSK)** packages — including modules, plugins, themes, and language packs.

Each package is managed as a **Git submodule**, enabling independent development, versioning, and distribution — while maintaining a unified structure for automation, updates, and releases.

## 🗂️ Repository Structure

Packages are organized by type:

```
packages/
├──languages
├──modules/
├──plugins/
└──themes/
```

Each subfolder contains official CSK components, many of which are private.

| Type      | Description                                  | Access |
| --------- | -------------------------------------------- | :----: |
| Languages | Translation packs                            |   🔒   |
| Modules   | Extend core functionality (e.g., Blog, Shop) |   🔒   |
| Plugins   | Add features or integrations                 |   🔒   |
| Themes    | Frontend Themes                              |   🔒   |

## 🛠️ Purpose

* Keep all official CSK extensions organized in one place.
* Provide a base for the CSK **in-app Marketplace**.
* Simplify updates, packaging, and distribution pipelines.
* Serve as a backend dependency hub for production builds.

## Automation
New packages register themselves automatically when they define:
- `CSK_NAME` variable → name of the package (e.g., `pages`).
- `CSK_TYPE` variable → type of the package (`module`, `theme`, etc.).
- `CSK_PAT` secret    → personal access token for communication.

> 🪄 This system allows decentralized development while maintaining a synchronized ecosystem.

---

## Example
| Type | Example Repo | CSK_NAME | CSK_TYPE | CSK_PAT | Added Under |
|------|--------------|-----------|----------|---------|-------------|
| Module | `csk-module-pages` | `pages` | `module` | `<secret>` | `packages/modules/pages` |
| Plugin | `csk-plugin-oauth` | `oauth` | `plugin` | `<secret>` | `packages/plugins/oauth` |
| Theme | `csk-theme-classic` | `classic` | `theme` | `<secret>` | `packages/themes/classic` |

---

> 🚀 CSK uses this monorepo to build update bundles and power its in-app marketplace.


## 🔗 Related Repositories

* [`csk-core`](https://github.com/ianhubnet) — Main CSK Framework *(Private)*
* [`csk-common`](https://github.com/ianhubnet/csk-common) — CSK Shared Assets *(Public)*
* [`csk-projects`](https://github.com/ianhubnet/csk-projects) — All CSK projects *(Public index)*

---

> This repository is part of the **Ianhub CSK ecosystem**. Most submodules are private, but their structure and organization are visible for transparency and documentation.
