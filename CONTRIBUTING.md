# 🤝 Contributing to Mini Market POS System

Thank you for considering contributing to the Mini Market POS System. Your help makes this project better.

## 🧾 Table of Contents

- [How to Contribute](#how-to-contribute)
- [Contribution Guidelines](#contribution-guidelines)
- [Pull Request Process](#pull-request-process)
- [Reporting Issues](#reporting-issues)
- [License](#license)
- [Copyright Notice](#copyright-notice)

---

## How to Contribute

1. Fork the repository
2. Clone your fork
   ```bash
   git clone https://github.com/NakiriFubuki/Pos_System.git
   ```
3. Navigate into the project directory
   ```bash
   cd Pos_System
   ```
4. Create a new branch
   ```bash
   git checkout -b feature/your-feature-name
   ```
5. Run the project locally with XAMPP
   - Place the folder under `C:\xampp\htdocs\Pos_System`
   - Start Apache and MySQL
   - Import the database (`import-database.bat` or `install-db.php`)
   - Visit `http://localhost/Pos_System/`
6. Make your changes
7. Test your changes
   - Admin and staff login
   - POS cart, member add, checkout
   - Receipt print / browser fallback
   - Notification bell badge clears after open
8. Commit your changes
   ```bash
   git commit -m "Add: a meaningful commit message"
   ```
9. Push to your branch
   ```bash
   git push origin feature/your-feature-name
   ```
10. Create a Pull Request

---

## Contribution Guidelines

- Keep the UI clean, modern, and consistent with the existing design
- Follow existing PHP / JS / CSS naming and folder structure
- Use prepared statements for all SQL
- Escape output with `e()` / `htmlspecialchars`
- Write clear, concise commit messages
- Update README screenshots when you change user-facing UI
- Do not commit secrets (`config/database.local.php`, live passwords, `.env`)

---

## Pull Request Process

- Create PRs from a feature branch (not directly from `main`)
- Describe what changed and why
- Include screenshots for UI changes when possible
- Wait for review / approval before merging
- Only maintainers should merge into the default branch

---

## Reporting Issues

Found a bug or have a feature idea? Please open an Issue and include:

- Browser / OS / PHP version
- Steps to reproduce
- Expected vs actual result
- Screenshots (if UI-related)

---

## Copyright Notice

This project and its UI are copyrighted content.

You may not copy, resell, or redistribute this project as your own commercial product without permission from the copyright holder.

Copyright (c) 2026 Eng Choon Hao. All Rights Reserved.

---

## License

This project is licensed under the [MIT Non-Commercial License](LICENSE).

Happy coding.
