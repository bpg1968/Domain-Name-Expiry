# Contributing to `exp`

Thank you for your interest in contributing to this project!
Please note that this project is **largely unmaintained**, and **pull requests, feature requests, and bug reports may not be addressed in a timely manner**.
However, if you would still like to contribute, please follow the guidelines below to ensure consistency and code quality.

## How to Contribute

### Bug Reports and Feature Requests

- Use GitHub Issues to report bugs or request features.
- Clearly describe the problem or feature.
- Include a sample run if relevant, and the version of your OS and shell.

### Code Contributions

If you'd like to submit code:

1. **Fork the repository**.
2. Create a new branch with a descriptive name:
   ```bash
   git checkout -b fix-whois-error
   ```
3. Make your changes.
4. Ensure your changes:
   - Follow POSIX-compliant shell scripting standards
   - Do not break any documented input/output behaviours
   - Include comments if functionality is not self-evident
5. **Test your changes** thoroughly.
6. Submit a pull request with a clear explanation of your changes.

### Style Guidelines

- Use 2-space indentation.
- Prefer readability over cleverness.
- Avoid external dependencies beyond `whois`, `date`, and `tput`.

## Code of Conduct

We expect all contributors to follow our [Code of Conduct](CODE_OF_CONDUCT.md). Be respectful and constructive in all interactions.

