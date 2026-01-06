# CLI Frameworks in Ruby (2026)

Ruby has a long history of excellent CLI tooling, primarily driven by the needs of the Rails ecosystem. However, the shift towards single-binary distribution in languages like Go has changed the landscape.

## Popular Frameworks

*   **[Thor](http://whatisthor.com/):** The grandfather of Ruby CLIs. Used by Rails itself. Excellent for subcommands and argument parsing but feels "classic" compared to modern declarative styles.
*   **[Dry-CLI](https://dry-rb.org/gems/dry-cli/):** Part of the `dry-rb` ecosystem. Offers a highly improved, object-oriented approach to defining commands. Great for complex, modular tools.
*   **[TTY Toolkit](https://ttytoolkit.org/):** A collection of independent gems (`tty-prompt`, `tty-box`, `tty-table`) rather than a monolith. It allows for "a la carte" construction of CLIs.
*   **[Commander](https://github.com/commander-rb/commander):** Bridging the gap between simple scripts and full CLI apps, focusing on a fluent API.

## Comparative Analysis: Ruby vs. Go (Charm/Cobra)

| Feature | Ruby (Thor/TTY) | Go (Cobra/Bubbletea) |
| :--- | :--- | :--- |
| **Distribution** | Requires Ruby runtime or complex packing (Tebako). | Compiles to single, static binary. |
| **Startup Time** | Slower (tens/hundreds of ms). | Instant (sub-10ms). |
| **Interactivity** | `tty-prompt` is excellent but imperative. | `Bubbletea` offers a declarative "Elm Architecture" for complex TUIs. |
| **Styling** | `pastel` / ANSI codes. | `Lipgloss` provides a CSS-like styling engine for terminals. |

**Benchmark Note:** For simple CRUD CLIs, Ruby's ease of writing beats Go's verbosity. For complex, persistent TUI dashboards (like `k9s` or `lazygit`), Go's performance and concurrency model are superior.
