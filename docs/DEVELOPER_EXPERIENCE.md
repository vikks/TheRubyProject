# Ruby Developer Experience (DevX) & Tooling

Ruby's "happiness first" philosophy still holds up, but tooling in Rust and Go has raised the bar for static analysis and speed.

## Tooling Landscape

*   **Debugging:** `debug` (the official debugger) has replaced `byebug` and offers decent integration. `pry` remains a favorite for REPL-driven development.
*   **LSP (Language Server Protocol):**
    *   **[Ruby LSP](https://github.com/Shopify/ruby-lsp):** The modern standard built by Shopify. Fast, robust, and powers the VS Code experience.
    *   **[Solargraph](https://solargraph.org/):** The older, community-driven alternative.
*   **Testing:** `RSpec` remains the arguably most expressive testing DSL in any language. `Minitest` offers a simpler, pure-Ruby approach.
*   **Packaging:** `Bundler` is still world-class, but the lack of a built-in "project manager" like `cargo` (which handles build, test, run, publish) is felt.

## Scaffolding & Code Gen

*   **Rails Generators:** Still the industry benchmark for scaffolding.
*   **Gaps:** We lack a "create-ruby-app" for non-Rails projects (e.g., CLI tools, Gems) that sets up the *entire* modern stack (LSP, Linting, GitHub Actions, Release workflow) in one command.
