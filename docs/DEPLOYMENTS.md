# Deployments & Server Management

Ruby's deployment story is evolving from "Capistrano scripts" to container-native, single-file orchestration.

## Key Tools

*   **[Kamal](https://kamal-deploy.org/):** (Formerly MRSK). The modern standard from 37signals.
    *   **Philosophy:** "No PaaS." Deploy containerized apps anywhere (AWS EC2, DigitalOcean, bare metal) with a single YAML config.
    *   **Features:** Zero-downtime deploys, rolling restarts, automatic SSL (Let's Encrypt).
    *   **Impact:** Democratizes "self-hosting" by removing the complexity of Kubernetes.
*   **[Capistrano](https://capistranorb.com/):** The legendary deployment automation tool. Still widely used for non-containerized "bare metal" setups.
*   **[Dokku](https://dokku.com/):** A Docker-powered mini-Heroku that you host yourself. Extremely popular in the Ruby community for small-to-medium apps.

## Comparative Trends

| Feature | Kamal | Kubernetes (Benchmark) | Heroku/Render (PaaS) |
| :--- | :--- | :--- | :--- |
| **Complexity** | Low (1 Config file). | High. | Zero. |
| **Cost** | Cost of VPS only. | High (Control plane). | Expensive markup. |
| **Lock-in** | None (Standard Docker). | Low. | High. |

## The "Kamal" Revolution

Kamal represents a shift back to "owning your infrastructure" without the overhead of enterprise orchestration. It fits perfectly with the Rails "One Person Framework" ideology.
