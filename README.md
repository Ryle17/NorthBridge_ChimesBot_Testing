# Northbridge Test College - fictional site for chatbot tests

Use when the real university site is unavailable. It has no emails or phone numbers anywhere, on purpose.

## Host it (pick one)
- Netlify Drop: drag this whole folder onto the Netlify Drop page; you get a public URL.
- GitHub Pages: push the folder to a repo and enable Pages.
Crawl starting from the home page (index.html).

## Tests
| Test | Setup | Ask | Expected |
|---|---|---|---|
| 8.6 | NEW bot whose ONLY source is this site URL | An unanswerable question, e.g. "What is data structures?" | Apology, then "You can also reach us at:" with a link to contact.html. No emails or phone numbers. |
| 10.2 | Add this site URL as a source | "When does the bell tower chime?" | 7:45 AM on school days |
| 10.2 | same | "When is the Founders' Day Quiz Bowl?" | First Friday of February |
| 10.3 | Site URL AND northbridge_admissions_circular.pdf in the same bot | "When is the application deadline?" | Does not pick one silently. Site says July 15, 2026; PDF says June 30, 2026. Should flag it or defer to the office. |
| 14.3 | Site URL | "Show me the BS Psychology page" | Link to program-psychology.html |
| 14.4 | Site URL | "Tell me about BS Psychology" | Psychology photo shown (not the banner) |
| 14.5 | Site URL | "Tell me about BS Library and Information Science" | Description (+ link). No apology, no image. |
| 14.6 | Site URL | "Do you have a photo of BS Library and Information Science?" | Says no photo is available. Must NOT show banner.png or another program's photo. |
| 14.7 | Site URL | "Show me photos of student life" | At most 2 images (the gallery page has 4) |
| 14.8 | Site URL | "Show me the campus" | campus.png (Main Building). Must NOT show banner.png. |

Re-sync the source after any change. Use a fresh conversation for each test.
