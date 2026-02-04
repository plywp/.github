![thumbnail](./thumbnail.png)
# PlyWP

PlyWP is an open-source WordPress **automation and management platform** built for developers, infrastructure engineers, and hosting systems that need scalable, programmable WordPress operations.

This org houses two main pieces of the PlyWP system:

* **panel** – A modern WordPress management control panel (built with Svelte)
* **plyorde** – A daemon written in Go that executes system-level WordPress tasks (site provisioning, web server and PHP management, database automation, etc.)
* **Plyserve** - A web server for plywp (currently not available)

PlyWP isn’t a typical “dashboard plugin.” It’s meant to treat WordPress as **managed infrastructure**, enabling reproducible, safe, automated workflows around WordPress environments.

---

## Why PlyWP Exists

Modern hosting isn’t about clicking buttons — it’s about *intent vs. execution*:

Traditional WordPress management tools focus on UI-driven interactions. PlyWP is designed to:

* Separate control (user intent, API calls, configuration) from execution
* Run real, system-level operations in a secure, auditable daemon
* Make WordPress controllable from scripts, CI/CD pipelines, and provisioning tools
* Reduce human error while improving repeatability and consistency

This approach turns WordPress into a **managed workload** instead of a manually operated site.

---

## What You’ll Find Here

### **panel**

A frontend that provides:

* Dashboard for WordPress site state
* Automation orchestration UI
* API interface for external tools
* Multi-site visibility

Built with modern front-end tooling for fast, reactive interfaces. ([GitHub][1])

---

### **plyorde**

The daemon that:

* Runs privileged tasks
* Manages system services (web server, PHP, databases)
* Executes installs, updates, and lifecycle tasks
* Logs and reports real state back to the panel

This keeps the sensitive, privileged operations separate from the UI layer, improving security and clarity. ([GitHub][1])

---

## Who It’s For

PlyWP targets:

* Hosting infrastructure teams
* Developers who treat WordPress as an automated service
* SaaS builders embedding WordPress into larger platforms
* Operators who need reproducible deployments

If your workflow needs predictable, scriptable WordPress management at scale, PlyWP is for you.

---

## Core Principles

PlyWP is built around these ideas:

* **Separation of Control & Execution**
  UI and API only describe *what should happen*; the daemon makes it happen.

* **Automation-First**
  All actions should be scriptable, repeatable, and auditable.

* **Explicit Operations**
  No hidden magic; what happens on the system is visible and intentional.

* **Infrastructure-Friendly**
  Designed for real server environments, not just manual use.

---

## Get Involved

This organization is early in development — APIs, workflows, and components will evolve as the project grows. Contributions, design feedback, and ideas are welcome.

---

## Powered By

PlyWP is crafted and maintained by **[Urixen](https://github.com/urixen-org)**, the principal engineer and visionary behind the project, with a focus on automation-native hosting systems and developer-friendly infrastructure tooling.
