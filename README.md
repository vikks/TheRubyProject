# TheRubyProject

**Modernizing the Ruby Ecosystem: A Comparative Study & Toolkit**

This project aims to aggregate tools, developer experiences, and workflows from modern ecosystems (Go, Rust, TypeScript, Python) and adapt them to Ruby. By leveraging AI and modern engineering practices, we aim to fill gaps in CLI development, UI components, and developer tooling.

## 📚 Ecosystem Overview

### 1. [CLI Frameworks](docs/CLI_FRAMEWORKS.md)
*Benchmark: Go (Cobra, Charm)*

| Tool | Type | Key Feature |
| :--- | :--- | :--- |
| **[Thor](http://whatisthor.com/)** | Framework | Subcommand parsing, used by Rails. |
| **[Dry-CLI](https://dry-rb.org/gems/dry-cli/)** | Framework | Object-oriented, modular command definition. |
| **[TTY Toolkit](https://ttytoolkit.org/)** | Library | Rich terminal components (Spinners, Tables, Prompts). |

### 2. [Web Frameworks](docs/WEB_FRAMEWORKS.md)
*Benchmark: Python (Django, FastAPI)*

| Tool | Type | Key Feature |
| :--- | :--- | :--- |
| **[Rails](https://rubyonrails.org/)** | Full-Stack | The standard. Hotwire, Solid Queue. |
| **[Hanami](https://hanamirb.org/)** | Full-Stack | Clean architecture, thread-safe. |
| **[Sinatra](http://sinatrarb.com/)** | Micro | Simple DSL for small apps/APIs. |

### 3. [UI Toolkits](docs/UI_TOOLKITS.md)
*Benchmark: React (Shadcn), Go (Bubbletea)*

| Tool | Category | Key Feature |
| :--- | :--- | :--- |
| **[Shadcn-Rails](https://github.com/shadcn-rails/shadcn-rails)** | Web | Tailwind + ViewComponent (Copy-pasteable). |
| **[Glimmer](https://github.com/glimmer-dsl-swt)** | Native GUI | Declarative DSL for cross-platform desktop apps. |
| **[Charm Ruby](https://github.com/charmbracelet/charm-ruby)** | TUI | Ruby port of Bubbletea/Lipgloss. |

### 3. [Developer Experience](docs/DEVELOPER_EXPERIENCE.md)
*Benchmark: Rust (Cargo), TS (LSP)*

| Tool | Category | Key Feature |
| :--- | :--- | :--- |
| **[Ruby LSP](https://github.com/Shopify/ruby-lsp)** | IDE | Modern Language Server by Shopify. |
| **[RSpec](https://rspec.info/)** | Testing | Expressive, behavior-driven testing DSL. |
| **[Debug](https://github.com/ruby/debug)** | Debugging | Native, fast debugger replacement for Byebug. |

### 4. [Deployments](docs/DEPLOYMENTS.md)
*Benchmark: Kubernetes, Docker Compose*

| Tool | Type | Key Feature |
| :--- | :--- | :--- |
| **[Kamal](https://kamal-deploy.org/)** | Orchestrator | Zero-downtime, container-native, no-PaaS. |
| **[Capistrano](https://capistranorb.com/)** | Automation | Classic, script-based server management. |

### 5. [Game Development](docs/GAME_DEVELOPMENT.md)
*Benchmark: Unity, Godot*

| Tool | Type | Key Feature |
| :--- | :--- | :--- |
| **[DragonRuby](https://dragonruby.org/)** | Engine | 2D, Hot-reload, Console support (Switch/PS4). |
| **[Gosu](https://www.libgosu.org/)** | Library | Mature, hardware-accelerated 2D graphics. |

### 6. [Cyber Security](docs/CYBER_SECURITY.md)
*Benchmark: Python (Scapy, Requests)*

| Tool | Category | Key Feature |
| :--- | :--- | :--- |
| **[Metasploit](https://www.metasploit.com/)** | Offensive | Premier pen-testing framework. |
| **[Brakeman](https://brakemanscanner.org/)** | Defensive | Static analysis for Rails security. |

### 7. [Embedded Systems](docs/EMBEDDED_SYSTEMS.md)
*Benchmark: C++, MicroPython*

| Tool | Type | Key Feature |
| :--- | :--- | :--- |
| **[mruby](https://mruby.org/)** | Language | Lightweight, embeddable Ruby for devices. |
| **[PicoRuby](https://github.com/picoruby/picoruby)** | Framework | Ruby for RP2040/Raspberry Pi Pico. |

### 8. [Data Science](docs/DATA_SCIENCE.md)
*Benchmark: Python (Pandas, Scikit-learn)*

| Tool | Type | Key Feature |
| :--- | :--- | :--- |
| **[Polars-ruby](https://github.com/ankane/polars-ruby)** | DataFrames | Blazing fast Rust-backed DataFrames. |
| **[Rumale](https://github.com/yoshoku/rumale)** | Machine Learning | Ruby version of Scikit-learn. |
| **[Torch.rb](https://github.com/ankane/torch-rb)** | Deep Learning | PyTorch power with Ruby syntax. |

### 9. [AI Integration](docs/AI_INTEGRATION.md)
*Benchmark: Python (LangChain)*

| Tool | Purpose | Key Feature |
| :--- | :--- | :--- |
| **[Langchain.rb](https://github.com/andreibondarev/langchainrb)** | Orchestration | Building agentic workflows in Ruby. |
| **[Ruby-OpenAI](https://github.com/alexrudall/ruby-openai)** | Client | Standard OpenAI API wrapper. |

## 🚀 [Ecosystem Gaps & Proposals](docs/ECOSYSTEM_GAPS.md)

We have identified key areas where Ruby can improve to match other modern languages:

*   **Distribution:** Single-binary compilation tools (like Go).
*   **TUI:** Event-driven architectures (Elm/Bubbletea style).
*   **Components:** A unified "GemCN" CLI for dropping in UI components.

---
*Generated on January 6, 2026*
