# Web Frameworks in Ruby

Ruby's web ecosystem is dominated by Rails, but a rich variety of alternatives exists, offering different paradigms from micro-services to clean architecture.

## Popular Frameworks

### The Monolith
*   **[Ruby on Rails](https://rubyonrails.org/):** The industry standard. Recent versions (7+) have aggressively pursued modern standards:
    *   **Hotwire:** HTML-over-the-wire for SPA-like responsiveness without complex JavaScript build steps.
    *   **Import Maps:** Delivering JavaScript modules directly to the browser, bypassing bundlers like Webpack.
    *   **Solid Queue / Solid Cache:** New, database-backed defaults for background jobs and caching, simplifying deployment.

### The Alternatives
*   **[Hanami](https://hanamirb.org/):** A robust, modern framework focusing on clean architecture, thread safety, and fast response times. It separates the domain logic from the delivery mechanism more strictly than Rails.
*   **[Sinatra](http://sinatrarb.com/):** The classic DSL for quickly creating web applications in Ruby with minimal effort. Great for simple APIs and microservices.
*   **[Roda](http://roda.jeremyevans.net/):** A routing tree web toolkit designed for high performance and reliability. It uses a unique routing tree approach that consumes less memory and is faster than linear routing.

## Comparative Trends

| Feature | Rails (The Omakase) | Hanami (The Architect) | Sinatra/Roda (The Minimalists) |
| :--- | :--- | :--- | :--- |
| **Philosophy** | Convention over Configuration. | Explicit over Implicit. | Simplicity and Speed. |
| **State Management** | ActiveRecord (Deeply integrated). | Repository Pattern (Decoupled). | Agnostic (Bring your own). |
| **Frontend** | Hotwire / Turbo (Default). | Agnostic / View Objects. | ERB / API-only. |

## Emerging Patterns

*   **HTML-over-the-Wire:** The Ruby community has largely rejected the "SPA-by-default" trend in favor of server-rendered HTML enhanced by lightweight JS (Turbo, Stimulus, Unpoly), reducing complexity.
*   **Component-Driven UI:** With `ViewComponent` and `Phlex`, even server-side Ruby is moving towards a component-based architecture similar to React/Vue.

## Deployment Frontiers: Serverless & Edge

While **Rails** remains the undisputed benchmark for rapid, stable development of long-running server applications, it currently faces challenges in **Serverless** and **Edge** environments.

*   **The Challenge:** Rails' "boot everything" approach leads to slower cold starts and higher memory usage, which fights against the constrained, ephemeral nature of AWS Lambda or Cloudflare Workers.
*   **Current State:** Tools like [Lamby](https://lamby.cloud/) bridge the gap, but lighter frameworks like **Sinatra** or **Roda** (or languages like Go/Rust/JS) are often preferred here.
*   **The Goal:** The ecosystem is working towards "modulith" loading and faster boot times to make Ruby a first-class citizen on the Edge.
