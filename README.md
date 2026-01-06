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

### 2. [UI Toolkits](docs/UI_TOOLKITS.md)
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

### 4. [AI Integration](docs/AI_INTEGRATION.md)
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
