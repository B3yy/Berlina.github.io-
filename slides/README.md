Slides README

What I added

- slides/slide-deck.md — The deck content in Markdown (one slide per '---' section).
- slides/speaker-notes.md — Compact speaker notes per slide.
- slides/reveal/index.html — A Reveal.js HTML preview you can open in a browser to present or print to PDF.

How to preview now (no install)

1. Open slides/reveal/index.html in your browser (use GitHub Pages or raw file preview).
   - If you view it locally, you may need a simple file server: python -m http.server 8000 then open http://localhost:8000/slides/reveal/index.html
2. Use arrow keys to navigate. Speaker notes are in the HTML <aside class="notes"> elements.

How to export a PPTX locally (two options)

Option A — Use Pandoc (recommended if you want a .pptx)

1. Install pandoc (https://pandoc.org/installing.html).
2. From the repo root run:

   pandoc slides/slide-deck.md -o assets/Berlina_Rasekgololo_Portfolio.pptx \
     --resource-path=.:slides --metadata title="Berlina Rasekgololo — Digital Product Portfolio"

3. The generated PPTX will be in assets/.

Option B — Use Reveal -> Print to PDF (then convert to PPTX manually)

1. Open slides/reveal/index.html in the browser.
2. File → Print → Save as PDF (choose A4 or Letter). This produces a PDF you can share.
3. If you need a PPTX, import the PDF into PowerPoint or use an online PDF→PPTX converter.

Notes

- Speaker notes are included in slides/speaker-notes.md and as <aside class="notes"> in the Reveal HTML.
- If you want, I can run the Pandoc conversion and commit the resulting PPTX to /assets/ — say "Convert & commit PPTX" and I will run that for you.

