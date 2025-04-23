# wp-impact-theme development setup
**Impact** is a versatile, classic/hybrid WordPress theme for startups and small businesses, by Berlin-based creative [web developer Ingo Steinke](https://www.ingo-steinke.de/), inspired by previous projects like the portfolio website for [sustainable stylist Tina Steinke (kleiderordnung)](https://kleiderordnung.berlin/) who had the idea of reusing elements of her website for purpose-driven startups. The Impact theme enables users to own and edit content without relying on costly third-party services. Although impact is a proprietary, commercial theme, that must be customized for individual use, we wanted to simplify our development process and make it possible to provide websites to startups and small businesses for affordable prices that respect their economic situation and their non-profit or impact-driven approach.

`wp-impact` is a white-label template that comes as-is with no guarantees. Please ask for customization prices!
As a developer interested in using this template, please contact us, and please submit issues and pull requests, or restrict your modifications to custom child themes. Impact is not available in the WordPress theme directory.

Customers get the free base theme plus an individual "child theme". Both themes must be installed; the child theme must be active.
The child theme's name should match the specific site name and purpose, e.g. `impact-child-mygreenbusiness`.

`wp-impact` obsoletes [`wp_cli_docker`](https://github.com/openmindculture/wp_cli_docker), [`wp_block_theme_child`](https://github.com/openmindculture/wp_block_theme_child), [`wp_template`](https://github.com/openmindculture/wp_template), and [`wp_template_opinionated`](https://github.com/openmindculture/wp_template_opinionated).

## Features (TODO)

* own and edit your content on a self-hosted server
* quick, simple, and energy-efficient
* accessible, responsive, progressive
* compatible for users of older devices and browsers
* optimized for visibility and search engine marketing
* prevent layout shift
* custom fonts and images
* classic customization
* classic/hybrid approach, no full site editing
* prevent/remove unnecessary data like emojis and duotone colors

## Customization

* theme customizer in wp-admin
* general settings
* child theme configuration files (`theme.json`, `style.css`, `functions.php`, custom blocks or block variations)

## Useful/recommended Plugins

Check if there is a preinstalled plugin where you can activate the necessary options.
Managed hosting, like offered by Bluehost, often comes with an additional, preinstalled plugin that includes most of the services mentioned below.
If not, try one of the suggested plugins. In most cases, the free plugin version should be sufficient for small businesses and personal projects. 

### Image Optimization

- reduce the size of uploaded image files
- create and provide optional image formats like `webp` and `avif`
- enable "lazy loading" for images that are not initially visible
- send caching headers to allow browsers to remember previous images

Plugins: Smush, Imagify, TinyPNG, ...

### Caching and Minimization (Minification)

- reduce the size of code files (HTML, JavaScript, CSS)
- store generated content to reduce costly database requests
- send caching headers to allow browsers to remember previous downloads

Plugins: W3 Total Cache, ...

### Marketing and Search Engine Optimization

- provide preview images and meta data for social sharing and search engines
- analyze your content and get tips for optimization

Plugins: Yoast SEO

### Backup and Restore

- make a copy of your website that you can restore if necessary,
- and that developers can use to set up a test (staging) server

Plugins: UpdraftPlus

### Security

- prevent malicious hacking attempts and denial-of-service attacks

Plugins: JetPack, WordFence, ...

### Contact Form / Communication

- allow users to contact you with a contact form
- prevent incoming unsolicited spam messages
- additional inbox to prevent lost e-mails

Plugins: Contact Form 7 + Flamingo (to store) + Akismet (for better spam protection)

## Development

`wp-impact-theme` contains an optional Docker development server setup.
The npm build step is also optional (but recommended), and so are the code quality tasks (eslint, stylelint, test).
There is no JavaScript/TypeScript transpiler, and no mandatory SCSS/PostCSS compilation.
All code should run without further modifications, at least in modern browsers.

In CSS, prefer mobile-first, responsive design, use relative units, font size clamp and container/content-based sizing, and prevent unnecessary pixel-based breakpoint media queries.
Make sure to respect accessibility queries like `prefers-reduced-motion` and ensure sufficient color contrast, font sizes, screen reader support, and keyboard navigation.

## Code Style

* all transpilations and build steps are optional
* surprise-less, consistent, reusable naming
* common parent theme slug (text domain) "impact" to simplify copy and paste between customer projects
* pragmatic coding and naming approach:
  * modern, PSR-compliant, PHP code to simplify automated linting and refactoring
  * modern CSS and JavaScript to simplify automated linting and refactoring
  * PHPDoc and JSDoc to enhance readability and code assistance
  * WordPress code style for functions (underscore) and class names (single dash) to simplify copy and paste from WordPress Codex documentation and AI-assisted suggestions

## Energy efficiency

Code style, reusability, and standards compliance should make so-called "artificial intelligence" (AI) assisted coding unnecessary in most cases.

As a developer, please try to reduce AI assistance to a minimum (e.g. one-line code completion suggestions, find errors, suggest refactoring). Please consult the official documentation (WordPress Codex, PHP.net, PSR coding standard etc.), static Q&A and developer community sites (StackOverflow, DEV, Reddit) and classic search engines (like Ecosia) instead of asking a virtual assistant, to prevent costly waste of energy!

As a designer and content creator, please optimize images and don't overuse video, to save bandwidth and prevent wasting energy!
