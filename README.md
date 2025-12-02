# RBAguila Personal Website

https://rbaguila.github.io

## Modern Portfolio Website

Personal portfolio showcasing Web2 and Web3 development projects with a modern dark/light theme design.

## Technology Stack

- **Frontend**: Modern CSS with dark/light theme support
- **Build System**: LESS preprocessor with direct compilation
- **JavaScript**: Vanilla JS with interactive features
- **Deployment**: GitHub Pages

## Development

### Initial Setup
```bash
npm install
```

### Build Commands

Due to Node.js v20 compatibility issues with Gulp 3, use these direct commands:

#### Compile LESS to CSS
```bash
npx lessc less/rbaguila.less css/rbaguila.css
```

#### Minify CSS
```bash
npx clean-css-cli -o css/rbaguila.min.css css/rbaguila.css
```

#### Minify JavaScript
```bash
npx terser js/rbaguila.js -o js/rbaguila.min.js -c -m
```

#### Full Build (all steps)
```bash
npx lessc less/rbaguila.less css/rbaguila.css && \
npx clean-css-cli -o css/rbaguila.min.css css/rbaguila.css && \
npx terser js/rbaguila.js -o js/rbaguila.min.js -c -m
```

### Development Server
```bash
npx serve .
```
Then visit http://localhost:3000

## Project Structure

- `/less/` - LESS source files
  - `rbaguila.less` - Main stylesheet
  - `variables.less` - Theme colors and variables
  - `mixins.less` - Reusable LESS mixins
- `/css/` - Compiled CSS (generated)
- `/js/` - JavaScript source and minified files
- `/img/portfolio/` - Project images
- `index.html` - Main HTML file

## Features

- Dark/Light theme toggle
- Typewriter effect on hero section
- Animated tech ticker
- Project filtering (Web3/Web2/Full-Stack/Backend)
- Skills-based project filtering
- Timeline journey visualization
- Interactive process workflow
- Fully responsive design
- Smooth scroll navigation

## Deployment

The site is automatically deployed via GitHub Pages from the `master` branch.

## License

MIT License
