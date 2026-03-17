# TKNIKA BRANDING & DESIGN SYSTEM

## Color Palette (STRICT)
* **Primary / Headers:** `#c1d10c` (Tknika Green) - Use for UI, PDF, and Sheets.
    * ❌ NEVER use the old Blue (`#0055a5`) or Lime (`#b1c42e`).
* **Text:** Black `#1c1c1a`.
* **Backgrounds:** White `#FFFFFF`.
* **Sub-Headers:** Light Gray (`#f2f2f2`) with Black text.

## UI & Web Rules
1. **Contrast:** Always ensure high contrast between Black text and White backgrounds.
2. **Accents:** Use Tknika Green (`#c1d10c`) for buttons, active states, and primary highlights.
3. **Typography:** Use modern sans-serif fonts like 'Inter' or 'Outfit' where possible.

## Google Sheets Rules
1. **Deep Clean Strategy:** Before applying any style, the code MUST clear all existing formats (`userEnteredFormat`) and unmerge cells to remove old artifacts.
2. **Dynamic Scanning:** Do NOT rely on hardcoded row indices for sheets other than the first. Scan Column A for keywords (e.g., "ZAINTZA PROZESUA", "HILABETEA") to apply Green background dynamically.
3. **Row 0 Sanctity:** The first row (Header) must ALWAYS be Black Background (`#1c1c1a`) with White Text (`#FFFFFF`).
4. **Column A1:** In "Grafikoak", force title to "ITURRI MOTA".

## PDF Layout Rules (WeasyPrint)
* **Tables:** Must use CSS `page-break-inside: avoid;` to prevent splitting rows across pages.
* **Header:** Must include the official Tknika logo.
* **Language:** Reports are strictly in EUSKARA.
