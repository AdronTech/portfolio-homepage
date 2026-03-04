# Portfolio Homepage

Small Hugo portfolio site using the Toha theme.

## Run locally

### 0) Initialize theme submodule (first clone only)

```bash
git submodule update --init --recursive
```

### 1) Prerequisites
- Hugo Extended (tested with `0.157.0`)
- Node.js (`v22.x` recommended)
- npm (`10.x` recommended)

Check tools:

```bash
hugo version
node -v
npm -v
```

### 2) Install dependencies (first run)

From the project root:

```bash
hugo mod tidy
hugo mod npm pack
npm install
```

### 3) Start local dev server

```bash
npm run dev
```

Open: http://localhost:1313

## Production build (local)

```bash
npm run build
```

## Notes
- If `hugo` is not found, install Hugo Extended first, then rerun the commands above.
- The deploy pipeline in `netlify.toml` uses the same Hugo + npm module workflow.
