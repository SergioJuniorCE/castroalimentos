# Castro Alimentos Website

This is the official website for Castro Alimentos, built with a modern, performant web stack focusing on speed and a great developer experience.

## 🚀 Tech Stack

- **Framework:** [Astro](https://astro.build/)
- **UI Library:** [React](https://react.dev/)
- **Styling:** [Tailwind CSS v4](https://tailwindcss.com/)
- **Components:** [shadcn/ui](https://ui.shadcn.com/) (Radix UI, Lucide React)
- **Deployment:** [Cloudflare Pages](https://pages.cloudflare.com/)
- **Linting & Formatting:** [Oxlint](https://oxc.rs/docs/guide/usage/linter.html) & [Oxfmt](https://oxc.rs/docs/guide/usage/formatter.html)

## 📁 Project Structure

```text
/
├── public/           # Static assets (images, fonts, etc.)
├── src/
│   ├── components/   # Astro and React UI components
│   ├── layouts/      # Page layouts
│   └── pages/        # Astro routing and pages
├── astro.config.mjs  # Astro configuration
├── package.json      # Dependencies and scripts
└── wrangler.jsonc    # Cloudflare Workers/Pages configuration
```

## 🧞 Getting Started

### Prerequisites
- [Bun](https://bun.sh/) installed on your machine.

### Installation

1. Clone the repository and install dependencies:
   ```sh
   bun install
   ```

2. Start the local development server:
   ```sh
   bun run dev
   ```
   The site should now be running locally.

## 📜 Available Scripts

| Command | Description |
| :--- | :--- |
| `bun run dev` | Starts the local dev server. |
| `bun run build` | Builds the production site to `./dist/`. |
| `bun run preview` | Builds the site and previews it locally using Cloudflare Wrangler. |
| `bun run deploy` | Builds the site and deploys it to Cloudflare Pages. |
| `bun run lint` | Runs the Oxlint linter to catch issues. |
| `bun run format` | Formats the codebase using Oxfmt. |
| `bun run format:check` | Checks if the codebase is properly formatted. |

## ☁️ Deployment

This project is configured to deploy to **Cloudflare Pages**. It uses the `@astrojs/cloudflare` adapter. 

You can deploy manually via the CLI using:
```sh
bun run deploy
```

Alternatively, push to the `master` or `main` branch to trigger the CI/CD deployment workflow via GitHub Actions (if configured in `.github/workflows/deploy.yml`).

## 🛠️ Code Quality

We use the [Oxc](https://oxc.rs/) toolchain for incredibly fast linting and formatting.
- **Linting:** Catch errors early by running `bun run lint`.
- **Formatting:** Ensure consistent code style by running `bun run format`.
