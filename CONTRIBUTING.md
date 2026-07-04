# Contributing to WizTree MCP Server

First off, thank you for considering contributing to the WizTree MCP Server! It's people like you that make the open-source community such an amazing place to learn, inspire, and create.

## How Can I Contribute?

### 1. 🐛 Reporting Bugs
If you find a bug, please create an issue on GitHub. Include as much detail as possible:
- Your operating system and Python version
- The exact error message or unexpected behavior
- Steps to reproduce the issue

### 2. ✨ Suggesting Enhancements
We love new ideas! If you have a feature request or a suggestion for a new "Skill" (agent workflow), please open an issue describing your idea and how it would benefit the project.

### 3. 🧠 Adding New Agent Skills
A huge part of this project is the `/skills` directory, which teaches AI agents how to safely manage storage. 
You can contribute by creating new `.md` files in the `skills/` directory that cover specific cleanup domains (e.g., `gaming_cache_cleanup.md`, `video_editing_cleanup.md`).

### 4. 💻 Code Contributions
Want to dive into the Python code? Great! Here is the standard workflow:

1. **Fork the repository** and clone it locally.
2. **Create a virtual environment**:
   ```bash
   python -m venv .venv
   .\.venv\Scripts\Activate
   pip install -r requirements.txt
   ```
3. **Create a new branch** for your feature or bug fix:
   ```bash
   git checkout -b feature/your-feature-name
   ```
4. **Make your changes** in `server.py` or other relevant files. Keep the code clean and well-documented.
5. **Commit your changes**:
   ```bash
   git commit -m "Add some feature"
   ```
6. **Push to the branch**:
   ```bash
   git push origin feature/your-feature-name
   ```
7. **Open a Pull Request** against the `main` branch.

## Code of Conduct
Please note that this project is released with a Contributor Code of Conduct. By participating in this project you agree to abide by its terms. Be respectful and constructive in your communications.

Thank you for helping make this project better! ❤️
