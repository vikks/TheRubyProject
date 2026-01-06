# UI Toolkits: GUI & TUI in Ruby

This is an area of significant divergence. Ruby has historically focused on the web (Rails), leaving the native GUI/TUI landscape fragmented compared to the component-driven architectures of React or the compiled efficiency of Rust/Go.

## GUI & TUI Libraries

### TUI (Terminal UI)
*   **[TTY Toolkit](https://ttytoolkit.org/):** The gold standard for Ruby. Rich components (spinners, bars, tables).
*   **[Charm Ruby](https://github.com/charmbracelet/charm-ruby):** A recent effort to port the Go Charm stack (Bubbletea, Lipgloss) to Ruby. Promising but less mature.

### Native GUI
*   **[Glimmer](https://github.com/glimmer-dsl-swt):** The most active cross-platform GUI library. Supports SWT (JRuby), LibUI (CRuby), and WebAssembly. It uses a declarative DSL.
*   **[Tk](https://github.com/ruby/tk):** The direct equivalent to Python's **Tkinter**. Formerly part of the standard library (pre-2.4), now a gem. Useful for legacy apps but less "modern" than Glimmer.
*   **[Shoes](http://shoesrb.com/):** The classic "tiny" toolkit. Great for teaching, less for production.

## The "Shadcn" Gap (Web Components)

Users accustomed to **shadcn/ui** (copy-pasteable, tailwind-based components) in the React world have spurred similar innovations in Ruby:

*   **[Shadcn-Rails](https://github.com/shadcn-rails/shadcn-rails):** A direct port. Generates ViewComponents with Tailwind classes that you own.
*   **[RailsUI](https://railsui.com/):** A premium and open-source library of pre-built ERB/ViewComponents.
*   **[Phlex](https://phlex.fun/) & [ViewComponent](https://viewcomponent.org/):** The foundational technologies enabling this shift. They bring "React-like" encapsulation to Rails views.
