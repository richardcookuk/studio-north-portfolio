# Studio North Portfolio

A text-led strategic communications portfolio for Richard Cook, built as a React and Vite web project in Manus.

## Requirements

- Node.js 20 or newer
- npm 10+ or pnpm 10+

## Install dependencies

Using npm:

```bash
npm install
```

Using the repository's preferred package manager:

```bash
pnpm install
```

## Run locally

Start the Vite development server:

```bash
npm run dev
```

Then open the local URL shown in the terminal, normally `http://localhost:3000`.

## Build for production

Create the production build with:

```bash
npm run build
```

The build command generates the Vite static site and the server bundle. The deployable static site is written to:

```text
dist/public
```

The additional server bundle is written to `dist/index.js` for the project's local production-server workflow. For **Cloudflare Pages**, use `npm run build` as the build command and set the output directory to `dist/public`.

To preview the Vite build locally:

```bash
npm run preview
```

To run the bundled local production server after building:

```bash
npm start
```

## Routes

The portfolio includes the following routes:

- `/`
- `/brings`
- `/expertise`
- `/working-with-richard`
- `/integrating`
- `/case-studies`
- `/testimonials`

A Cloudflare Pages `_redirects` file is included under `client/public/` so client-side routes resolve to the application shell when deployed as a static site.

## Quality checks

Run the TypeScript check with:

```bash
npm run check
```

Format the source with:

```bash
npm run format
```

## Notes

Environment files and generated build output are intentionally excluded from version control. The project uses the existing Manus frontend runtime configuration during local development; no secrets should be committed to this repository.
