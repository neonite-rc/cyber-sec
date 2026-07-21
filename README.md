# Cyber-Sec

Cybersecurity experiments and vulnerability demonstrations. Exploring how file formats, protocols, and systems can be abused for unexpected behavior.

## Projects

### PDF-Snake
A proof-of-concept demonstrating PDF field object abuse to render a monochrome grid with keyboard input handling — effectively a game engine inside a PDF.

**Fork of:** [pdftris by ThomasRinsma](https://github.com/ThomasRinsma/pdftris)

**Mechanism:** Abuses PDF field objects to render a monochrome grid, combined with keystroke-entry in a text field to receive inputs. Works in PDFium (Chromium-based browsers) and PDF.js (Firefox).

**Why this matters:** Demonstrates that PDFs are not passive documents — they contain a Turing-complete scripting environment that security teams often overlook.

**Controls:**
- Arrow keys to control the snake
- Ensure the input field is focused

**Tested in:**
- Chrome/Chromium (PDFium)
- Firefox (PDF.js)

## Stack
PDF specification, JavaScript (PDF), Python (generation), forensic analysis

## Status
✅ PDF-Snake functional — tested in Chrome and Firefox PDF viewers.

## Future
- [ ] PDF malware analysis sandbox
- [ ] Protocol fuzzing experiments
- [ ] Web application security assessments

## Credits
- **Original concept**: [Tetris in a PDF](https://th0mas.nl/2025/01/12/tetris-in-a-pdf) by [Th0mas](https://th0mas.nl)

## License
MIT
