# Cyber Security in Ruby

Ruby is a powerhouse in the infosec world, largely due to Metasploit, but also plays a critical role in securing its own web ecosystem.

## Key Tools & Frameworks

### Offensive Security (Red Team)
*   **[Metasploit Framework](https://www.metasploit.com/):** The world's most used penetration testing framework is written in Ruby. It allows for developing and executing exploit code against a remote target machine.
*   **[Ronin](https://ronin-rb.dev/):** A Ruby toolkit for security research and development. It provides a platform for writing exploits and tools.

### Application Security (Blue Team)
*   **[Brakeman](https://brakemanscanner.org/):** A static analysis security vulnerability scanner for Ruby on Rails applications. It checks for SQL injection, XSS, and more.
*   **[Bundler-Audit](https://github.com/rubysec/bundler-audit):** Patch-level verification for Gems. Checks your `Gemfile.lock` against a database of known security vulnerabilities.
*   **[Rack Attack](https://github.com/rack/rack-attack):** Middleware for blocking & throttling abusive requests (DoS protection, Brute-force defense).

## The State of Security

Ruby's dynamic nature makes static analysis harder than in Rust/Go, but tools like **Brakeman** are mature and effective. The community is highly proactive about CVE disclosures (via the Ruby Advisory Database).
