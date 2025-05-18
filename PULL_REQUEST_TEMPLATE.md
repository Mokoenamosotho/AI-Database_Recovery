# Creating a pull request template

pr_template_path = Path("/mnt/data/hospital-dbms/.github/PULL_REQUEST_TEMPLATE.md")

pr_template_content = """# 📦 Pull Request Template

## Description
<!-- Provide a brief summary of the changes you made -->

## Related Issue
<!-- Link to the issue that this PR addresses (e.g., Closes #12) -->

## Type of Change
- [ ] 🐛 Bug Fix
- [ ] ✨ New Feature
- [ ] 🧹 Code Cleanup / Refactor
- [ ] ✅ Tests Added/Updated
- [ ] 📄 Documentation Update

## Checklist
- [ ] Code compiles without errors
- [ ] All tests pass locally
- [ ] I've added unit tests where needed
- [ ] I've updated relevant documentation/comments
- [ ] My changes follow the contribution guidelines

## Screenshots / Additional Context
<!-- Add screenshots or context if applicable -->
"""

# Write the PR template file
pr_template_path.write_text(pr_template_content)

pr_template_path
