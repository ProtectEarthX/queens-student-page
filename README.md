# queens-student-page
website:  https://protectearthx.github.io/queens-student-page/

## CISC 121 Code Review Checklist (SMART Feedback)

### 1. Functionality
- In `index.html` line 35, the `mailto:` link uses the placeholder `21ds56@queensu.ca`. Replace it with your real email and click it to confirm it opens a mail client without console errors. Fix before merge.

### 2. Clarity
- In `index.html` line 22, the image alt text says “Your Name portrait”. Update it to the actual name (e.g., “Steve Page portrait”) and confirm a screen reader reads the updated text. Fix before merge.
- In `index.html` lines 27–30, the course list uses “Course One/Two/Three/Four”. Replace these with the real course names so someone can understand the list without extra context; verify by rereading the list. Fix before merge.

### 3. Structure
- In `index.html` lines 18–35, the About, Courses, and Contact blocks are not wrapped in semantic sections. Wrap each block in a `<section>` element and keep the current heading hierarchy (h1 then h2s). Complete in the next update.

### 4. Maintainability
- In `style.css` line 10, `h2` uses the hard-coded color `#8B4513`. Move this to a CSS variable (for example, `--heading`) in `:root` and use it in `h2`; verify the page colors remain unchanged. Fix before merge.

### 5. Performance
- `profile.jpeg` is about 984 KB. Compress/resize it to under 500 KB and confirm the file size with `ls -l` while keeping the image clear. Fix before publishing.

### 6. Security & Privacy
- In `index.html` line 35, the email address exposes a student ID. If this is personal, replace it with an alias or a contact form and confirm the old address is no longer in the HTML. Fix before public release.

### 7. Documentation
- `README.md` has no setup instructions. Add 2–3 steps (for example, “open `index.html`” or `python -m http.server`) and confirm a new user can view the site locally within 2 minutes. Add in the next update.

### 8. Testing
- After updates, test the layout at 320px and 768px widths (DevTools) and confirm there is no horizontal scrolling; if there is, add a small-screen media query to reduce `main` margins/padding. Complete before merge.
