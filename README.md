# Code-to-Slide Generator

A tool to generate high-quality images from code snippets, formatted for Google Slides (16:9).

## 🚀 Features
- **16:9 Ratio:** Dimensions set to 1920x1080 for perfect slide integration.
- **Side-by-Side:** Support for two code blocks in a single image.
- **Line Selection:** Extract specific line ranges (e.g., `10-25`).
- **Languages:** Python and C support (automatic file extension detection).

## 🛠 Dependencies
The script requires the following Python packages:
- `pygments`
- `playwright` (with `playwright install chromium`)

## 💻 Usage

### Single Snippet
```bash
code-slides hello.py --lines1 1-15 -o output.png
```

### Side-by-Side Snippets
```bash
code-slides before.c --file2 after.c -o comparison.png
```

### Specific Lines
```bash
code-slides main.py --lines1 10-20 --file2 test.py --lines2 5-15 -o summary.png
```
