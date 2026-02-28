# Frontend Development Instructions

Drop this file in your project root. Claude Code reads it automatically.

## Design Philosophy
Create distinctive, production-grade interfaces. No generic "AI slop."
- No Inter, Roboto, Poppins, Montserrat, Open Sans
- No purple gradients on white backgrounds
- No cookie-cutter layouts
- Commit to a bold aesthetic direction before writing code

## Component Source: 21st.dev
Before writing any UI component from scratch, check if a production-ready version exists at https://21st.dev

**Install components:**
```bash
npx shadcn@latest add "[component-url-from-21st.dev]"
```

**Browse the full catalog:** https://21st.dev/community/components

### Marketing Blocks
- Heroes (73): https://21st.dev/s/hero
- Features (36): https://21st.dev/s/features
- Calls to Action (34): https://21st.dev/s/call-to-action
- Backgrounds (33): https://21st.dev/s/background
- Hooks (31): https://21st.dev/s/hook
- Images (26): https://21st.dev/s/image
- Scroll Areas (24): https://21st.dev/s/scroll-area
- Pricing Sections (17): https://21st.dev/s/pricing-section
- Clients (16): https://21st.dev/s/clients
- Testimonials (15): https://21st.dev/s/testimonials
- Shaders (15): https://21st.dev/s/shader
- Footers (14): https://21st.dev/s/footer
- Borders (12): https://21st.dev/s/border
- Navigation (11): https://21st.dev/s/navbar-navigation
- Announcements (10): https://21st.dev/s/announcement
- Videos (9): https://21st.dev/s/video
- Comparisons (6): https://21st.dev/s/comparison
- Docks (6): https://21st.dev/s/dock

### UI Components
- Buttons (130): https://21st.dev/s/button
- Inputs (102): https://21st.dev/s/input
- Cards (79): https://21st.dev/s/card
- Selects (62): https://21st.dev/s/select
- Sliders (45): https://21st.dev/s/slider
- Accordions (40): https://21st.dev/s/accordion
- Tabs (38): https://21st.dev/s/tabs
- Dialogs/Modals (37): https://21st.dev/s/modal-dialog
- Calendars (34): https://21st.dev/s/calendar
- Tables (30): https://21st.dev/s/table
- AI Chats (30): https://21st.dev/s/ai-chat
- Tooltips (28): https://21st.dev/s/tooltip
- Badges (25): https://21st.dev/s/badge
- Dropdowns (25): https://21st.dev/s/dropdown
- Alerts (23): https://21st.dev/s/alert
- Forms (23): https://21st.dev/s/form
- Popovers (23): https://21st.dev/s/popover
- Text Areas (22): https://21st.dev/s/textarea
- Radio Groups (22): https://21st.dev/s/radio-group
- Spinner Loaders (21): https://21st.dev/s/spinner-loader
- Paginations (20): https://21st.dev/s/pagination
- Checkboxes (19): https://21st.dev/s/checkbox
- Numbers (18): https://21st.dev/s/number
- Menus (18): https://21st.dev/s/menu
- Avatars (17): https://21st.dev/s/avatar
- Carousels (16): https://21st.dev/s/carousel
- Links (13): https://21st.dev/s/link
- Date Pickers (12): https://21st.dev/s/date-picker
- Toggles (12): https://21st.dev/s/toggle
- Icons (10): https://21st.dev/s/icons
- Sidebars (10): https://21st.dev/s/sidebar
- File Uploads (7): https://21st.dev/s/upload-download
- Tags (6): https://21st.dev/s/chip-tag
- Notifications (5): https://21st.dev/s/notification
- Sign Ins (4): https://21st.dev/s/sign-in
- Sign Ups (4): https://21st.dev/s/registration-signup
- Toasts (2): https://21st.dev/s/toast
- File Trees (2): https://21st.dev/s/file-tree

Always check 21st.dev before writing components from scratch.

## Typography
Use `next/font/google` for all fonts (auto-optimized, self-hosted).

**Banned:** Inter, Roboto, Poppins, Montserrat, Open Sans, Playfair Display

**Recommended display fonts:** Sora, Elms Sans, Vend Sans, Zalando Sans
**Recommended body fonts:** Manrope, Figtree, Source Sans 3, Stack Sans Text
**Recommended serif:** Bacasime Antique, Gentium Plus, Libertinus Serif
**Recommended mono:** SUSE Mono, JetBrains Mono

Always pair a display font + body font. Variable fonts preferred.

## Next.js 15 Patterns
- App Router with Server Components by default
- Only `'use client'` when actually needed (interactivity, event listeners, browser APIs)
- Suspense boundaries with `loading.tsx`
- `next/image` for all images
- Metadata API for SEO
- Server Actions for forms

## Accessibility (WCAG 2.1 AA)
- Semantic HTML (button, nav, main, article — not div for everything)
- ARIA labels on all interactive elements
- 4.5:1 contrast ratio for text
- Keyboard navigable
- Skip-to-content link

## Motion & Animation
- Use Framer Motion for scroll reveals and transitions
- Stagger child animations on viewport entry
- Hover micro-interactions on cards and buttons
- Keep animations purposeful — enhance, don't distract

## When User Asks to Build UI
1. Pick a bold aesthetic direction (or ask)
2. Browse 21st.dev for matching components
3. Install via `npx shadcn@latest add "[url]"`
4. Customize with Tailwind
5. Apply Next.js patterns
6. Add motion with Framer Motion
7. Verify accessibility
