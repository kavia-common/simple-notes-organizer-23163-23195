# Ocean Notes (Astro)

A simple, modern notes app built with Astro. No backend required—your notes are stored locally in your browser (localStorage).

Ocean Notes follows the Ocean Professional design: primary #2563EB, secondary/success #F59E0B, error #EF4444, background #f9fafb, surface #ffffff, text #111827. The UI uses subtle gradients, rounded corners, and soft shadows.

## Features

- Create, edit, and delete notes
- Local persistence with localStorage
- Search/filter notes
- Keyboard shortcuts:
  - N: new note
  - Ctrl/Cmd+S: save current note
  - Delete: delete selected note
- Export and import notes as JSON
- Clean Ocean-themed UI with smooth transitions

## Getting Started

1. Install dependencies:
   npm install

2. Run the dev server:
   npm run dev

3. Build for production:
   npm run build

4. Preview the build:
   npm run preview

## Project Structure

- src/pages/index.astro – App page and client logic
- src/layouts/Layout.astro – Global layout and metadata
- src/styles/global.css – Ocean Professional theme and app styles
- src/components/ThemeToggle.astro – Light/Dark toggle

## Notes Format

Notes are stored under the localStorage key ocean_notes_v1 as an array of:
{
  id: string,
  title: string,
  content: string,
  updatedAt: number // epoch ms
}

## Accessibility

- Navigable note items (Enter/Space to select)
- ARIA live regions for status updates
- High-contrast accents and focus states
