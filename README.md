# IntelliToggle

A Nuxt 3 + Tailwind CSS web app for smart feature flagging and AI-driven rollout management.

## URL Link

[https://intellitoggle-azure.vercel.app/](https://intellitoggle-azure.vercel.app/)

## Getting Started

### Prerequisites

- Node.js v18 or newer
- npm v9 or newer

### Setup

1. **Clone the repository:**
   ```bash
   git clone <your-repo-url>
   cd intellitogle
   ```
2. **Install dependencies:**
   ```bash
   npm install
   ```
3. **Prepare Nuxt build artifacts:**
   ```bash
   npx nuxi prepare
   ```
4. **Run the development server:**
   ```bash
   npm run dev
   ```
   The app will be available at [http://localhost:3000](http://localhost:3000).

### Build for Production

```bash
npm run build
```

### Generate Static Site

```bash
npm run generate
```

## Project Structure

- `app/` — Main Vue app, assets, and CSS
- `components/` — Reusable Vue components
- `layouts/` — App layouts (header, footer, etc.)
- `pages/` — Route-based pages
- `public/` — Static assets (images, etc.)

## Tech Stack

- [Nuxt 3](https://nuxt.com/) — Vue framework
- [Tailwind CSS v4](https://tailwindcss.com/) — Utility-first CSS
- [Vite](https://vitejs.dev/) — Build tool

## Tradeoffs

### Fast Iteration vs. Maintainability

Using Tailwind utilities directly in Vue templates allows for rapid prototyping and quick style changes without leaving the component file. However, this can result in long class strings that are harder to maintain, refactor, and debug as the project grows.

### Pixel-Perfect Design vs. Brittleness

Tailwind's extensive utility classes provide precise control over styling, enabling pixel-perfect designs that match exact specifications. However, this approach can make the codebase brittle to changes in design requirements or responsive breakpoints, requiring updates across multiple components.

## With More Time

1. **Component Library**: Create a reusable component library with consistent design tokens (colors, spacing, typography) to improve maintainability and speed up future development.

2. **Performance Optimizations**: Implement lazy loading for images, code splitting for routes, and bundle analysis to reduce initial load times and improve user experience.

## Customization

- Edit `tailwind.config.js` to adjust theme, colors, and breakpoints.
- Add new pages in `pages/` and components in `components/`.

## Troubleshooting

- If you see errors about missing `.nuxt` or build artifacts, run:
  ```bash
  npx nuxi prepare
  ```
- For Tailwind CSS IntelliSense, ensure you have the [Tailwind CSS IntelliSense VS Code extension](https://marketplace.visualstudio.com/items?itemName=bradlc.vscode-tailwindcss) installed.
