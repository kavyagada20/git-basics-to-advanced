# 📝 Git Commit Messages Best Practices

---

## 📌 Overview

Commit messages are essential for maintaining a **clear and meaningful project history**.

👉 Good commit messages help:
- Understand changes quickly  
- Improve collaboration  
- Debug issues efficiently  

---

## 🎯 Why Good Commit Messages Matter

- Makes history readable  
- Helps team collaboration  
- Simplifies debugging  
- Improves code reviews  

---

➡️ Next Step

Continue to:

👉 02-branching-strategy.md

## 🧱 Structure of a Commit Message

```bash
<type>: <short summary>

<optional detailed description>
🔤 Common Commit Types
Type	Description
feat	New feature
fix	Bug fix
docs	Documentation changes
style	Code formatting (no logic change)
refactor	Code improvement
test	Adding/updating tests
chore	Maintenance tasks
✨ Examples
feat: add user authentication
fix: resolve login button issue
docs: update installation guide
refactor: optimize API response handling
🧠 Writing Good Commit Messages
✅ Do:
Use present tense
Keep it short and clear
Be descriptive
Use proper type prefixes
❌ Avoid:
Vague messages like "update"
Long unnecessary descriptions
Mixing multiple changes in one commit
📏 Recommended Rules
Limit title to ~50 characters
Use lowercase for type
Separate title and description with a blank line
🧪 Example (Full Format)
feat: add payment integration

Integrated Razorpay API for handling online payments.
Added validation and error handling.
🧠 Conventional Commits

Follow standard format:

<type>(optional-scope): description

Example:

feat(auth): add JWT authentication
🔍 Benefits of Conventional Commits
Standardized history
Better automation (CI/CD, changelogs)
Easier collaboration
⚠️ Common Mistakes
Writing unclear messages
Skipping commit types
Combining unrelated changes
🎯 Summary
Write clear, concise commit messages
Follow a consistent format
Use commit types for clarity
Keep history clean and readable