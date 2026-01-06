# Ecosystem Gaps & Proposals

To match the developer experience of Go, Rust, and TS, the Ruby ecosystem should target these specific areas:

| Area | Gap | Proposal / Project Idea |
| :--- | :--- | :--- |
| **Distribution** | "It works on my machine" vs. Single Binary. | **Ruby-Packer-NG:** A streamlined, zero-config tool to wrap a Ruby CLI into a cross-platform binary (bundling the interpreter) without 15 minutes of compilation. |
| **TUI Architecture** | Imperative spaghetti vs. Elm Architecture. | **RubyTea:** A fully robust, event-loop driven TUI framework for Ruby that mimics Bubbletea's Model-Update-View pattern. |
| **Component Library** | Fragmentation in ViewComponents. | **GemCN:** A centralized CLI tool to "add" components (Buttons, Modals) to *any* Ruby project (Hanami, Sinatra, Rails) using Phlex or standard ERB. |
| **Data Science** | Python dominance. | **Ruby-Polars:** Continued investment in high-performance dataframes to make Ruby a viable "glue" language for ML workflows, even if the heavy lifting is C++/Rust. |
| **Serverless / Edge** | Rails cold-start times are too high for Lambda/Edge. | **Ruby-on-Edge:** A community initiative to standardize sub-500ms boot times and lighter memory footprints for major frameworks, potentially leveraging CRuby 3.3+ optimizations or Wasm. |
