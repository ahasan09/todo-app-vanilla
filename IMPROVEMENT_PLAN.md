# Improvement Plan: Hasan-ToDo-App

## Overview
Single-file vanilla JS todo app. Functional but uses ES5 patterns, has no tests, no build pipeline, and limited accessibility.

## Improvements

### Code Quality
- Refactor from a single-file IIFE to ES modules (`import`/`export`) — eliminates the global namespace and enables tree-shaking
- Convert to TypeScript for type safety on task objects
- Add ESLint + Prettier for consistent code style
- Split `app.js` into logical modules: `storage.js`, `ui.js`, `tasks.js`

### Testing
- Add Jest unit tests for core logic (add/edit/delete/filter tasks, localStorage read/write)
- Add Playwright e2e tests for the main user flows

### Accessibility
- Ensure all interactive elements have proper ARIA labels
- Add keyboard navigation support (add task on Enter, delete on Delete key)
- Verify color contrast meets WCAG AA

### Features
- Add due dates and priority levels for tasks
- Add drag-and-drop reordering
- Add dark mode toggle

### DevOps
- Add a `package.json` with Vite for bundling and a dev server
- Add GitHub Actions CI to run linting and tests on every push
