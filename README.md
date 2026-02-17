# 📖 Mahiru's OCR
**A Professional AI-Powered Workspace for Manga & Manhua Extraction.**

Mahiru's OCR is a high-performance desktop application built for scanlators and readers. It leverages state-of-the-art Vision AI to extract text with surgical precision while respecting the complex reading orders of Japanese, Korean, and Chinese comics.

## ✨ Key Features
- **Multi-Language Mastery:** Optimized prompts for Japanese (Vertical/RTL), Korean (Webtoon style), Chinese, and English.
- **Pro-Workspace Layout:** Toggleable sidebars and dynamic grids for a focused editing experience.
- **Smart Queue System:** Concurrent processing using multiple API keys with automatic 30s cooldown rotation and error handling.

## 🚀 Getting Started
1. **Download:** Grab the latest Releases from the [Releases](https://github.com/VAlBHAV-AGARWAL/Mahiru-OCR/releases) page.
2. **Install:** Run the installer. If Windows shows a warning, click "More Info" -> "Run Anyway".
3. **Activate:** Open the app, go to **Settings (Gear Icon)**, and enter your provided Email and Serial Key.
4. **Configure:** Add your Gemini, OpenAI, or Claude API keys in the **Manage API Keys** section.

## 🛠 Requirements
- **OS:** Windows 10/11 (x64 or x86).
- **Internet:** Required for license activation and ocr process.
- **AI Access:** You must provide your own API keys for Gemini, OpenAI, or Anthropic.

---

# Mahiru OCR - User Manual

Mahiru OCR is a desktop OCR tool for scanned pages, manga/comics, and very long images (webtoons or stitched pages). It helps you extract text, clean it up in a structured editor, and export the final result as plain text.
Mahiru OCR uses your own API keys (`Gemini` / `OpenAI` / `Claude`). All OCR costs depend on your provider and plan.

---

## 1. First-Time Setup

1. Activate your license in the `Activation` tab.
2. Open `OCR > Control Panel > Keys` and add at least one API key.
3. Optional: open `OCR > Control Panel > Legends` and adjust text markers.
4. Choose:
   - **Model:** `Gemini Flash Latest` (Recommended)
   - **Language:** your document language

---

## 2. Quick Start (Normal Pages)

1. Load a folder with images.
2. Set:
   - **Batch Size:** `1x` or `2x` (recommended)
   - **Speed Mode:** `Normal` (stable)
3. Click **Start OCR**.
4. Review results in the editor.
5. Fix mistakes if needed.
6. Click **Save Results** to export text.

You can re-run OCR on the same images anytime with different settings.

---

## 3. API Keys & Cost

Mahiru uses your own provider keys. Cost depends on provider and plan.

- Add multiple keys to improve throughput.
- Paid keys can be scheduled more aggressively.
- OCR cannot start if no active key is available.

---

## 4. Choosing Model & Speed

### Recommended Model

`Gemini Flash Latest` is currently the most stable option for most users.

### Other Providers

`OpenAI` and `Claude` are available, but behavior may vary by model and provider updates.

### Speed Mode

- **Normal:** safer and more stable.
- **Fast:** quicker processing, but more cooldown/rate-limit risk.

---

## 5. Batch Size - How to Pick

Batch size controls how many pages/segments are sent in one request.

- **1x - 2x (Recommended):** best quality/stability balance.
- **3x (Advanced):** faster, quality may drop on complex pages.
- **4x - 5x (Experimental):** only if you accept trade-offs; consistency can drop.

If quality matters most, stay at **1x** or **2x**.

---

## 6. Normal Pages vs Long Images

### Normal Pages

- Keep **Long-Image Slicing** OFF.
- Run OCR normally.

### Long Images (Webtoon / Stitched)

- Turn **Long-Image Slicing** ON.
- Choose slicing mode (Smart or Direct).

---

## 7. Long-Image Slicing: Smart vs Direct

### Smart Mode (Try First)

Smart mode tries to cut at natural empty spaces/gutters. It is usually better for mixed or complex layouts.

It may struggle when:

- cut height is too small (often below ~`2000px`), or
- there are no clean gutters.

### Direct Mode

Direct mode cuts at a fixed height.

Enable **Continue Slice** to carry leftover pixels into the next image. This helps avoid boundary text loss.

---

## 8. Smart Stitch (For Difficult Pages)

Use Smart Stitch when slicing keeps cutting text badly.

It can:

- combine multiple images into one long image,
- then split again with cleaner boundaries before OCR.

Save and reuse **Stitch Presets** for consistent scans.

---

## 9. Text Import & Alignment

You can import text from:

- another OCR tool, or
- scripts/novels/translations.

Workflow:

1. Paste text or upload `.txt` / `.docx`.
2. Set **Page Divider** to split text into chunks.
3. Enable **Auto Align** to map chunks to images.

If chunk count and image count do not match, Mahiru warns you so you can adjust divider settings or ignore extras.

---

## 10. Legends (Text Types & Presets)

Legends define markers for text types in Blocks mode:

- Dialogue
- Thoughts
- SFX
- Narration
- Small text/signs

You can customize legends and save/load presets per project.

---

## 11. Editing: Blocks Mode vs Raw Mode

- **Blocks Mode:** structured editing by text type, best for manga/comics formatting.
- **Raw Mode:** plain text editing, best for quick cleanup.

---

## 12. Exporting Results

Export output as plain text.

For best quality, review and edit before exporting.

---

## 13. Quality & Performance Tips

- Smaller batch sizes usually improve quality.
- Paid keys usually improve speed.
- For very large images:
  - enable slicing,
  - avoid very small cut heights.
- If output looks wrong:
  - lower batch size,
  - switch Smart/Direct slicing,
  - use Smart Stitch,
  - re-run OCR with adjusted settings.

---
*Developed with ❤️ for the Manga community.*
*Contact Here - [Discord](https://discord.gg/jWN46cmJZK) Server.
