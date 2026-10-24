# Project Instructions

<!-- ideaz-preview-contract -->

This project is edited through IDEaz, which previews it by mounting the working
tree in a WebView and transpiling JSX/TS in the browser with Babel. There is no
build step and no dev server: whatever is on disk is what renders.

Practical consequences for an agent editing this repository:

- Edit source files directly. Do not add a bundler step or expect one to run.
- Bare specifiers (`react`, `react-dom`, and the common ecosystem libraries)
  resolve through a bundled import map. Adding a dependency to `package.json`
  does not make it importable in the preview.
- Vite-only features are unsupported: `import.meta.env`, HMR, and glob / `?raw`
  / `?url` imports.
