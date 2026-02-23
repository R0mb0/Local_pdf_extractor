# Local pdf extractor

[![Codacy Badge](https://app.codacy.com/project/badge/Grade/a2abb5ace1a94c4ca36659f26b05b098)](https://app.codacy.com/gh/R0mb0/Local_pdf_extractor/dashboard?utm_source=gh&utm_medium=referral&utm_content=&utm_campaign=Badge_grade)
[![pages-build-deployment](https://github.com/R0mb0/Local_pdf_extractor/actions/workflows/pages/pages-build-deployment/badge.svg)](https://github.com/R0mb0/Local_pdf_extractor/actions/workflows/pages/pages-build-deployment)
[![Maintenance](https://img.shields.io/badge/Maintained%3F-yes-green.svg)](https://github.com/R0mb0/Local_pdf_extractor)
[![Open Source Love svg3](https://badges.frapsoft.com/os/v3/open-source.svg?v=103)](https://github.com/R0mb0/Local_pdf_extractor)
[![MIT](https://img.shields.io/badge/License-MIT-blue.svg)](https://opensource.org/license/mit)
[![Donate](https://img.shields.io/badge/PayPal-Donate%20to%20Author-blue.svg)](http://paypal.me/R0mb0)

A modern client-side tool to bulk convert PDFs into a unified document. Features drag-and-drop, auto dark mode, and multi-language support. Built with React and PDF.js.

<div align="center">

## [👉 Click here to test the page! 👈](https://r0mb0.github.io/Local_pdf_extractor/)

[![01.png](https://github.com/R0mb0/Local_pdf_extractor/blob/main/ReadMe_Imgs/01.png?raw=true)](https://r0mb0.github.io/Local_pdf_extractor/)

[![02.png](https://github.com/R0mb0/Local_pdf_extractor/blob/main/ReadMe_Imgs/02.png?raw=true)](https://r0mb0.github.io/Local_pdf_extractor/)

</div>

---

<h2>🚀 Features</h2>
    <ul>
        <li><strong>Bulk Extraction</strong>: Drag & drop unlimited PDF files at once.</li>
        <li><strong>Smart Formatting</strong>: Heuristic algorithms attempt to reconstruct paragraphs and detect headers (H1, bold text) from the raw PDF stream.</li>
        <li><strong>Multi-Format Output</strong>: Export merged content as:
            <ul>
                <li><strong>Markdown (.md)</strong>: Perfect for LLM context or note-taking apps.</li>
                <li><strong>HTML (.html)</strong>: Ready for web use.</li>
                <li><strong>Plain Text (.txt)</strong>: Raw data.</li>
            </ul>
        </li>
        <li><strong>Runs entirely in the browser</strong>: No server, no backend, no installation required.</li>
        <li><strong>Privacy-first</strong>: Your files never leave your computer.</li>
        <li><strong>Auto-Adaptive UI</strong>: Automatically detects system language (EN/IT) and Theme (Light/Dark).</li>
    </ul>

  <h2>🛠️ How it works</h2>
  <ol>
      <li><strong>Upload your PDF(s)</strong> via the drag & drop interface.</li>
      <li>The tool uses <strong>PDF.js</strong> to parse the binary data of each file locally.</li>
      <li>It extracts text items and sorts them by coordinates (Y/X) to reconstruct the reading order.</li>
      <li>An algorithm analyzes font size and spacing to determine line breaks and headers.</li>
      <li><strong>Turndown</strong> converts the structure into clean Markdown (if selected).</li>
      <li><strong>Download</strong> the single, unified document containing all data.</li>
  </ol>

  <h2>🏆 What makes it special?</h2>
  <ul>
      <li><strong>Zero-Dependency Setup (Offline)</strong>: Can be run offline by simply opening <code>index.html</code> if libraries are downloaded locally.</li>
      <li><strong>Header & Format Detection</strong>: Unlike standard "Select All > Copy" methods, this tool tries to preserve the semantic structure of the document (Titles, Bold text).</li>
      <li><strong>Infinite Scalability</strong>: Since it runs on your client machine, you are not limited by server upload caps or timeouts.</li>
  </ul>

  <h2>💡 Why use this tool?</h2>
  <ul>
      <li><strong>LLM Context Preparation</strong>: Quickly merge 20+ PDFs into one Markdown file to feed into ChatGPT or Claude.</li>
      <li><strong>Research Consolidation</strong>: Combine multiple papers into a single searchable text file.</li>
      <li><strong>Privacy</strong>: Sensitive documents remain on your device.</li>
  </ul>

  <h2>🔒 Privacy & Security</h2>
  <ul>
      <li><strong>All processing is done locally</strong> in your browser.</li>
      <li><strong>No file is sent to any server</strong>.</li>
      <li><strong>No data is stored</strong>; memory is cleared upon page refresh.</li>
  </ul>

  <h2>⚡ Getting Started</h2>

  <h3>Online</h3>
  <p>Simply visit the <a href="https://r0mb0.github.io/Local_pdf_extractor/">Demo Page</a>.</p>

  <h3>Local Installation (Offline)</h3>
  <ol>
      <li><strong>Clone this repository</strong>.</li>
      <li>Ensure the library files (<code>react.js</code>, <code>pdf.js</code>, etc.) are in the root folder.</li>
      <li>Open <code>index.html</code> in your browser.</li>
      <li>Toggle the comments in the <code>&lt;head&gt;</code> of the HTML file to switch from CDN to Local libraries.</li>
  </ol>

  <h2>✨ Limitations & Notes</h2>
  <ul>
      <li><strong>Text-Based PDFs Only</strong>: This tool extracts text layers. It does <strong>not</strong> perform OCR. If your PDF is a scanned image (without a text layer), use my <a href="https://github.com/R0mb0/PDF_accessibility_fixer">PDF Accessibility Fixer</a> instead.</li>
      <li><strong>Complex Layouts</strong>: While it handles standard documents well, complex multi-column layouts or tables might be extracted linearly.</li>
      <li><strong>Formatting</strong>: The reconstruction is heuristic; it may not be pixel-perfect compared to the original visual layout.</li>
  </ul>

  <h2>📖 License</h2>
  <p>MIT License. See <a href="https://www.google.com/search?q=LICENSE">LICENSE</a> for details.</p>

  <h2>🙏 Credits & Inspiration</h2>
  <ul>
      <li><a href="https://github.com/mozilla/pdf.js">PDF.js</a> for parsing.</li>
      <li><a href="https://github.com/mixmark-io/turndown">Turndown</a> for HTML-to-Markdown conversion.</li>
      <li><a href="https://reactjs.org/">React</a> & <a href="https://tailwindcss.com/">TailwindCSS</a> for the UI.</li>
  </ul>


<a href="https://github.com/R0mb0/Crafted_with_AI">
  <picture>
    <source media="(prefers-color-scheme: dark)" srcset="https://github.com/R0mb0/Crafted_with_AI/blob/main/Badge/SVG/CraftedWithAIDark.svg">
    <source media="(prefers-color-scheme: light)" srcset="https://github.com/R0mb0/Crafted_with_AI/blob/main/Badge/SVG/NotMadeByAILight.svg">
    <img alt="Not made by AI" src="https://github.com/R0mb0/Crafted_with_AI/blob/main/Badge/SVG/NotMadeByAIDefault.svg">
  </picture>
</a>
