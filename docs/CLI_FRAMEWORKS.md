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
| **Interactivity** | `tty-prompt` is excellent but imperative. | `Bubbletea` offers a declarative "Elm Architecture" for complex TUIs. |
| **Styling** | `pastel` / ANSI codes. | `Lipgloss` provides a CSS-like styling engine for terminals. |

---

### Performance & Distribution Note
Certain performance characteristics (startup time, memory footprint) and distribution models (single-binary compilation) are inherently language-dependent and are out of scope for this specific framework comparison. For efforts to bridge these gaps in Ruby (e.g., single-binary packing), see [Ecosystem Gaps & Proposals](ECOSYSTEM_GAPS.md).
