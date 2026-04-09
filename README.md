# 📧 MBOX to Clean TXT

> Strip the clutter from your email exports and get a clean text file ready for [NotebookLM](https://notebooklm.google/).

## 🚀 Live Demo

**[Open the converter →](https://adminnooot.github.io/mboxtotxt/)**

No install needed. Everything runs in your browser — your emails never leave your device.

## What it does

MBOX files exported from Gmail, Thunderbird, or Apple Mail are packed with headers, HTML markup, base64-encoded attachments, and other noise. This tool:

- **Parses** the `.mbox` file and splits it into individual emails
- **Strips** HTML tags, inline styles, scripts, and encoded attachments
- **Decodes** quoted-printable and base64 text content
- **Handles** MIME multipart messages (prefers plain text, falls back to HTML→text)
- **Removes** reply quotations (`>`), signature blocks, and forwarded-message clutter
- **Outputs** a clean, readable `.txt` file with just the content that matters

## How to use

1. Open the [live demo](https://adminnooot.github.io/mboxtotxt/)
2. Drag & drop your `.mbox` file (or click to browse)
3. Toggle options:
   - **Keep email headers** — include From, To, Date, Subject
   - **Separator between emails** — visual divider line
   - **Sort by date** — chronological order
4. Click **Convert to Clean TXT**
5. Preview the result and click **Download Clean TXT**

## Privacy

100% client-side. No data is uploaded anywhere. The file is read and processed entirely in your browser using JavaScript.

## Exporting your MBOX

| Provider     | How to export                                                 |
|-------------|---------------------------------------------------------------|
| **Gmail**    | [Google Takeout](https://takeout.google.com/) → select Mail   |
| **Thunderbird** | Right-click folder → Save As → `.mbox`                    |
| **Apple Mail** | Mailbox → Export Mailbox                                    |

## Running locally

Just open `index.html` in any modern browser — no build step or server required.

```bash
git clone https://github.com/adminnooot/mboxtotxt.git
cd mboxtotxt
open index.html    # macOS
# or: xdg-open index.html   # Linux
# or: start index.html       # Windows
```

## License

MIT