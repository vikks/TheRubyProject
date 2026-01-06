# CLI Frameworks in Ruby (2026)

## 1. The Benchmark: Modern CLI Standards
Current industry standards for CLI development are often defined by ecosystems like:
*   **Go (Cobra/Charm):** Characterized by single-binary distribution, declarative TUI (Elm architecture), CSS-like styling (Lipgloss), and auto-generated documentation.
*   **Node.js (Ink/Oclif):** Features React-based TUI rendering (Ink), plugin architectures, and optimized startup times.

## 2. Ruby Ecosystem Status
*   **Current State:** Ruby tooling emphasizes *developer ergonomics* for defining logic and parsing arguments (Thor/Dry-CLI). Visual presentation (TUI architecture) and distribution models differ from compiled counterparts.
*   **Observation:** Ruby is widely used for scripting and automation tasks, while complex, interactive "dashboard" CLIs are more commonly associated with the benchmarked ecosystems.

## 3. Library-Specific Analysis

### [Thor](http://whatisthor.com/) vs. [Cobra](https://github.com/spf13/cobra) (Go) / [Oclif](https://oclif.io/) (Node)
*Context: Standard scaffolding frameworks.*

| Feature | Thor (Ruby) | Benchmark (Cobra/Oclif) | Comparison |
| :--- | :--- | :--- | :--- |
| **Argument Parsing** | ✅ Robust (Flags, Subcommands). | ✅ Robust. | Functionally comparable. |
| **Doc Generation** | ⚠️ Basic help text. | ✅ Auto-gen Man pages & Markdown docs. | Cobra/Oclif natively generate static documentation formats; Thor relies on runtime help output. |
| **Completion** | ⚠️ Manual/Limited. | ✅ Auto-gen Shell completion scripts. | Benchmark tools often generate shell scripts (Bash/Zsh/Fish) automatically from command definitions. |
| **Plugins** | ❌ None standard. | ✅ Oclif has a robust plugin system. | Oclif provides a standardized protocol for external plugins; Thor does not enforce a specific plugin architecture. |

### [TTY Toolkit](https://ttytoolkit.org/) vs. [Charm Bubbletea](https://github.com/charmbracelet/bubbletea) / [Ink](https://github.com/vadimdemedes/ink)
*Context: Interactive UI layers.*

| Feature | TTY (Ruby) | Benchmark (Bubbletea/Ink) | Comparison |
| :--- | :--- | :--- | :--- |
| **Architecture** | ⚠️ Imperative. | ✅ Declarative (Elm/React). | TTY primarily uses a synchronous "ask/wait" pattern. Benchmark libraries use state-driven, render-loop patterns. |
| **Layout** | ⚠️ Manual calculation. | ✅ Flexbox/CSS-like engines. | Benchmark libraries include layout engines (e.g., Yoga) to automatically handle dimensions and padding. |
| **Events** | ❌ Blocking input. | ✅ Async Event Loop. | Benchmark libraries typically handle asynchronous keyboard, mouse, and window resize events. |

### [Dry-CLI](https://dry-rb.org/gems/dry-cli/) vs. [Clap](https://github.com/clap-rs/clap) (Rust)
*Context: Architecture-focused builders.*

| Feature | Dry-CLI (Ruby) | Benchmark (Clap) | Comparison |
| :--- | :--- | :--- | :--- |
| **Type Safety** | ✅ Strong (via Dry-Types). | ✅ Strong (Rust static typing). | Both implement type constraints, one at runtime and the other at compile time. |
| **Modularity** | ✅ Registry-based. | ✅ Macro/Struct-based. | Dry-CLI uses a dynamic registry for command composition; Clap uses static struct definitions. |

## 4. Potential Ecosystem Additions
The following features, present in benchmark tools, are currently not standard in the Ruby CLI ecosystem:

1.  **State-Driven TUI Loop:** A library implementing the `Model -> View -> Update` pattern (similar to Bubbletea).
2.  **Universal Completion Generator:** Tooling to parse Thor/Dry-CLI definitions and output standard shell completion scripts.
3.  **Decoupled Style Builder:** A CSS-like string builder for ANSI, independent of IO operations (similar to Lipgloss).

## 5. Ruby's Distinct Characteristics
Ruby CLI development offers specific traits compared to the benchmarks:

*   **DSL Expressiveness:** Ruby's syntax allows for command definitions that are often more concise than equivalent implementations in Go or Rust.
*   **Runtime Dynamism:** Ruby CLIs can modify command structures at runtime (e.g., conditional commands based on configuration) without recompilation.
*   **REPL Integration:** Development workflows often benefit from `Pry` or `IRB` integration for interactive debugging and inspection.

---
### Performance Note
See [Ecosystem Gaps](ECOSYSTEM_GAPS.md) for details on Startup Time and Binary Distribution.
