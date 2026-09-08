from pathlib import Path

path = Path("/mnt/data/README.md")
text = path.read_text(encoding="utf-8")

# Remove private/direct contact items and portfolio.
text = text.replace("-   **Email:** fwahlah18@gmail.com\n", "")
text = text.replace("-   **Phone:** (+92) 306 4238780\n", "")
text = text.replace("-   **Portfolio:** https://bit.ly/4zLCBaB\n", "")

# Hyperlink LinkedIn in GitHub Markdown.
text = text.replace("-   **LinkedIn:** Faryal Nasir", "-   **LinkedIn:** [Faryal Nasir](https://www.linkedin.com/in/faryalnasir007/)")

# Make the Markdown itself cleaner and intentionally designed for GitHub rendering.
text = text.replace(
    "# Faryal Nasir\n\n**Full-Stack Engineer \\| .NET · React · Python · AI & Agentic\nDevelopment**",
    """<div align="center">

# Faryal Nasir

### Full-Stack Engineer · .NET · React · Python · AI & Agentic Development

</div>

---"""
)

# Replace section headings with a restrained GitHub-friendly visual treatment.
repls = {
    "## Contact": "## 🔗 Connect",
    "## Work Experience": "## 💼 Work Experience",
    "## Education": "## 🎓 Education",
    "## Skills": "## 🛠️ Technical Skills",
    "## Languages": "## 🌐 Languages",
    "## References": "## 📌 References",
}
for a, b in repls.items():
    text = text.replace(a, b)

# Add separators before major sections for better GitHub layout.
for heading in ["## 💼 Work Experience", "## 🎓 Education", "## 🛠️ Technical Skills", "## 🌐 Languages", "## 📌 References"]:
    text = text.replace("\n" + heading, "\n\n---\n\n" + heading)

path.write_text(text, encoding="utf-8")
print("Updated README.md with GitHub-friendly Markdown design and requested privacy/link changes.")
