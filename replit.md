# LUXE STUDIO

A premium, responsive salon and barbershop website template for local businesses in India.

## Run & Operate

- `pnpm --filter @workspace/luxe-studio run dev` — run the website preview
- `pnpm --filter @workspace/luxe-studio run typecheck` — typecheck the website
- `PORT=5000 BASE_PATH=/ pnpm --filter @workspace/luxe-studio run build` — build the website

## Stack

- pnpm workspaces, Node.js 24, TypeScript 5.9
- Frontend: React + Vite
- Styling: CSS with responsive layouts and reduced-motion support
- Icons: Lucide React
- No backend, database, payment gateway, or appointment persistence in version one

## Where things live

- `artifacts/luxe-studio/src/config.ts` — source of truth for salon name, contact details, location, hours, services, INR prices, gallery, stylists, testimonials, FAQs, and social links
- `artifacts/luxe-studio/src/App.tsx` — single-page layout, navigation, booking request behavior, service tabs, testimonial controls, and FAQ
- `artifacts/luxe-studio/src/index.css` — theme tokens, responsive layout, typography, animations, and focus states
- `artifacts/luxe-studio/index.html` — SEO title, description, Open Graph, Twitter card metadata, and favicon

## Architecture decisions

- All salon-specific content is kept in one editable config file so the template can be reused for another client without searching through the component.
- Booking actions are intentionally paused for the demo and show a launch-status message instead of opening a redirect.
- The app is frontend-only by design. No payment, auth, or appointment database is included in version one.
- Demo imagery uses commercially permissible Unsplash image URLs and every image includes descriptive alt text.

## Product

LUXE STUDIO presents a fictional premium salon and barbershop with:

- Sticky desktop and mobile navigation
- Hero, salon story, service categories with INR prices, gallery, stylists, demo testimonials, visit details, FAQ, and footer
- Accessible booking area with a professional launch-status message
- Click-to-call phone and Google Maps directions links
- Responsive layouts for mobile, tablet, and desktop

## User preferences

- Keep the code beginner-friendly and easy to customize for local salon and barbershop clients.
- Clearly label testimonials as demo content and booking as unavailable until launch.

## Gotchas

- Replace the demo contact details, photos, testimonials, and business copy in `src/config.ts` before using the template for a real salon.
- Re-enable booking only after adding the client's approved launch workflow.
- The website uses remote Unsplash imagery; download client-owned images locally if a client needs a fully self-contained deployment.

## Pointers

- Website artifact: `artifacts/luxe-studio`
- Reusable business content: `artifacts/luxe-studio/src/config.ts`
- See the `pnpm-workspace` skill for workspace structure, TypeScript setup, and package details
