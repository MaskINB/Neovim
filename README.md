# Neovim Configuration

This is a Neovim configuration optimized for React/Next.js development.

## React/Next.js Development Setup

### LSP Support
- **TypeScript/JavaScript**: `tsserver` with inlay hints enabled
- **CSS/Tailwind**: `cssls`, `tailwindcss`
- **HTML**: `html`

### Formatting & Linting
- **Prettier**: Code formatting for JS/TS, HTML, CSS, JSON, etc.
- **ESLint**: JavaScript/TypeScript linting
- **Stylelint**: CSS/SCSS linting

### Debugging
- **JavaScript/TypeScript**: `js-debug-adapter` for DAP debugging
- **Python**: `debugpy` for Python debugging

### Keymaps for React/Next.js

#### NPM Scripts
- `<leader>nr`: Run `npm run dev` (development server)
- `<leader>nb`: Run `npm run build` (production build)
- `<leader>ns`: Run `npm start` (production server)
- `<leader>nt`: Run `npm test` (run tests)
- `<leader>ni`: Run `npm install` (install dependencies)
- `<leader>nl`: Run `npm run lint` (run linter)
- `<leader>np`: Open `package.json`

#### Debugging
- `<F5>`: Start/Continue debugging
- `<F1>`: Step into
- `<F2>`: Step over
- `<F3>`: Step out
- `<leader>b`: Toggle breakpoint
- `<leader>B`: Set conditional breakpoint
- `<F7>`: Toggle debug UI

#### LSP
- `gd`: Go to definition
- `gr`: Find references
- `gI`: Go to implementation
- `<leader>D`: Type definition
- `<leader>rn`: Rename symbol
- `<leader>ca`: Code actions
- `K`: Hover documentation
- `<leader>th`: Toggle inlay hints

### VS Code Tasks
You can also use VS Code tasks for npm scripts:
- `Ctrl+Shift+P` → "Tasks: Run Task" → Select npm script

### Installation
1. Install required tools:
   ```bash
   :MasonInstall typescript-language-server prettierd js-debug-adapter
   ```

2. For React/Next.js projects, ensure you have:
   - Node.js installed
   - `package.json` with scripts defined
   - ESLint and Prettier configured (optional)

### Notes
- ESLint diagnostics are handled by your project's ESLint configuration
- Prettierd is used for faster formatting
- TypeScript inlay hints are enabled by default
- Debugging works for both JavaScript and TypeScript files

### File Types Supported
- `.js`, `.jsx`, `.ts`, `.tsx`
- `.json`, `.html`, `.css`, `.scss`
- `.md`, `.yaml`, `.toml`

### Treesitter Parsers
- `javascript`, `typescript`, `tsx`, `jsx`
- `html`, `css`, `json`, `yaml`
- `markdown`, `bash`, `lua`, `python`