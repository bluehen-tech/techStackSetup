# BlueHenDSSATechStack

Workshop materials for the DSSA Member Portfolio Workshop - Git & GitHub Basics for Contributing to the DSSA Website.

🔗 **Repository**: [https://github.com/bluehen-tech/techStackSetup](https://github.com/bluehen-tech/techStackSetup)  
🌐 **Live Site**: [https://bluehen-tech.github.io/techStackSetup/](https://bluehen-tech.github.io/techStackSetup/)

## 📖 About This Repository

This repository contains the workshop guide (`index.qmd`) that teaches DSSA members how to contribute to the UD-DSSA website using Git and GitHub. The guide is written in Quarto (`.qmd` format) and rendered as HTML for display on GitHub Pages. The rendered site is available at [https://bluehen-tech.github.io/techStackSetup/](https://bluehen-tech.github.io/techStackSetup/).

## 🛠️ Prerequisites

To edit and render this workshop guide, you'll need:

- **Quarto** - A scientific and technical publishing system
- **Git** - Version control (covered in the workshop!)
- **A code editor** - VS Code or Cursor (recommended)

## 📦 Installing Quarto

### Windows

1. Go to [quarto.org/download](https://quarto.org/download)
2. Download the Windows installer
3. Run the installer and follow the prompts
4. Restart your terminal/VS Code after installation

### macOS

1. Go to [quarto.org/download](https://quarto.org/download)
2. Download the macOS installer (`.pkg` file)
3. Double-click to install
4. Restart your terminal/VS Code after installation

### Linux

```bash
# Using apt (Ubuntu/Debian)
sudo apt-get update
sudo apt-get install -y quarto

# Or download from quarto.org/download
```

### Verify Installation

Open a terminal and run:

```bash
quarto --version
```

You should see something like `1.4.x` or higher.

## ✏️ Making Changes

1. **Clone this repository** (if you haven't already):
   ```bash
   git clone https://github.com/bluehen-tech/techStackSetup.git
   cd techStackSetup
   ```

2. **Open the project in VS Code/Cursor**

3. **Edit `index.qmd`** - This is the main workshop guide file
   - It's written in Markdown with some Quarto-specific features
   - You can preview changes as you work

4. **Preview your changes** (optional but recommended):
   ```bash
   quarto preview index.qmd
   ```
   This opens a live preview in your browser that updates as you edit.

## 🎨 Rendering the HTML

To generate the final HTML file that will be displayed on GitHub Pages:

1. **Open a terminal** in VS Code/Cursor (`` Ctrl + ` ``)

2. **Make sure you're in the project directory**:
   ```bash
   cd techStackSetup
   ```

3. **Render the HTML**:
   ```bash
   quarto render index.qmd
   ```

4. **Check the output**: You should see `index.html` and an `index_files/` folder created/updated

5. **Preview locally** (optional):
   ```bash
   quarto preview index.qmd
   ```
   Or simply open `index.html` in your browser.

## 🚀 Publishing to GitHub Pages

The rendered `index.html` file is automatically displayed on the GitHub Pages site. Here's the workflow:

1. **Make your changes** to `index.qmd`

2. **Render the HTML**:
   ```bash
   quarto render index.qmd
   ```

3. **Commit both files**:
   ```bash
   git add index.qmd index.html index_files/
   git commit -m "Update workshop guide: [describe your changes]"
   ```

4. **Push to GitHub**:
   ```bash
   git push origin main
   ```

5. **GitHub Pages will automatically update** - Usually takes a few minutes. View the live site at [https://bluehen-tech.github.io/techStackSetup/](https://bluehen-tech.github.io/techStackSetup/)

## 📝 Workflow Summary

Here's the typical workflow for updating the workshop guide:

```bash
# 1. Make sure you're up to date
git pull origin main

# 2. Make your changes to index.qmd
# (Edit in VS Code/Cursor)

# 3. Preview your changes (optional)
quarto preview index.qmd

# 4. Render the HTML
quarto render index.qmd

# 5. Commit and push
git add index.qmd index.html index_files/
git commit -m "Your commit message"
git push origin main
```

## 🎯 Quick Reference

### Common Quarto Commands

- `quarto render index.qmd` - Render HTML from the QMD file
- `quarto preview index.qmd` - Live preview with auto-refresh
- `quarto --version` - Check Quarto version
- `quarto check` - Verify Quarto installation and dependencies

### File Structure

```
techStackSetup/
├── index.qmd          # Source file (edit this!)
├── index.html         # Rendered output (auto-generated)
├── index_files/       # Supporting files (auto-generated)
└── README.md          # This file
```

## 💡 Tips

- **Always render before committing** - Make sure `index.html` is up to date
- **Preview locally first** - Use `quarto preview` to catch formatting issues
- **Commit both `.qmd` and `.html`** - The source file and rendered output should be in sync
- **Check GitHub Pages** - After pushing, wait a few minutes and check the live site at [https://bluehen-tech.github.io/techStackSetup/](https://bluehen-tech.github.io/techStackSetup/)

## 🆘 Troubleshooting

### "quarto: command not found"
- Make sure Quarto is installed and added to your PATH
- Restart your terminal/VS Code after installing Quarto
- Verify with `quarto --version`

### "Rendering failed"
- Check for syntax errors in `index.qmd`
- Make sure all required Quarto extensions are installed
- Try running `quarto check` to diagnose issues

### "HTML not updating on GitHub Pages"
- Make sure you committed both `index.html` and `index_files/`
- Check GitHub Pages settings in your repository
- Wait a few minutes - GitHub Pages can take time to update

## 📚 Resources

- **Quarto Documentation**: [quarto.org/docs](https://quarto.org/docs)
- **Quarto Guide**: [quarto.org/docs/guide](https://quarto.org/docs/guide)
- **GitHub Pages**: [docs.github.com/pages](https://docs.github.com/pages)

## 🤝 Contributing

1. Fork this repository
2. Create a branch for your changes
3. Make your edits to `index.qmd`
4. Render the HTML with `quarto render index.qmd`
5. Commit your changes (both `.qmd` and `.html`)
6. Push and create a pull request

---

**Questions?** Reach out to the DSSA team!
