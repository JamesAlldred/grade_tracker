Grade Tracker

A single-file, offline grade tracking tool for university coursework. Built as vanilla HTML, CSS, and JavaScript with no build step, no framework, and no external dependencies using Claude.

What it does
Tracks modules, assignments, and grades across all four years of a degree
Calculates credit-weighted averages per year, falling back to a simple mean when credit data is unavailable
Applies editable, per-year degree weightings to compute an overall classification estimate
Shows live summary cards that update as data changes
Includes a "what-if" slider mode for modelling hypothetical future grades
Supports excluding specific modules or assignments from calculations
Auto-saves with a debounce delay, so edits persist without manual saving
Offers dark mode with Auto, Light, and Dark options
Includes an Advanced view with toggleable column visibility
Organises non-degree modules (e.g. extracurricular or non-credit courses) in a separate Other Courses section, structured as Folder > Course > Part, each with editable Steps and a colour-coded Type
Files
File	Purpose
grade_tracker.html	Main working version, with real grade data baked in
grade_tracker_blank.html	Distributable version with no personal data, for sharing or starting fresh
grade_tracker_handoff.md	Development notes and context, updated after each editing session
Usage

Open grade_tracker.html directly in a browser. No server or installation required.

For live-reload while editing in VS Code, use the Live Server extension: right-click grade_tracker.html and select "Open with Live Server."

Note: data is stored in the browser's localStorage, which is tied to the file's origin. Known quirks:

Works reliably in Chrome
file:// access in Firefox does not persist localStorage correctly (unresolved, browser-level limitation)
Moving the file to a different sync path (e.g. into or out of OneDrive) can change its origin and disconnect it from previously saved data
Development notes

This project is developed through small, scoped, additive edits rather than full rewrites. Any change to grade_tracker.html is mirrored in grade_tracker_blank.html where applicable, and grade_tracker_handoff.md is kept up to date as a running log of decisions and in-progress work.

Status

Actively maintained. See grade_tracker_handoff.md for the current state and next steps.
