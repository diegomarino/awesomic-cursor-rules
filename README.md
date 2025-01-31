# Cursor Rules Documentation

[![Cursor](https://img.shields.io/badge/Cursor-Rules-blue.svg)](https://cursor.sh)
[![Format](https://img.shields.io/badge/Format-MDC-green.svg)](https://cursor.sh)

This directory contains standardized rules and best practices for development using Cursor IDE. These rules are designed to maintain consistency, improve code quality, and streamline development processes across projects.

## Available Rules

### Code and Documentation

- [`code-style-javascript.mdc`](rules/code-style-javascript.mdc) - JavaScript and TypeScript coding standards
- [`comments-javascript.mdc`](rules/comments-javascript.mdc) - Documentation and commenting guidelines
- [`readme-md.mdc`](rules/readme-md.mdc) - README file structure and content standards
- [`contributing-md.mdc`](rules/contributing-md.mdc) - Contributing guidelines for collaborators

### Development Workflow

- [`git-conventions.mdc`](rules/git-conventions.mdc) - Git workflow and hooks standards
- [`environment-variables.mdc`](rules/environment-variables.mdc) - Environment configuration practices
- [`testing-standards-jest.mdc`](rules/testing-standards-jest.mdc) - Testing guidelines with Jest

### Operations and Security

- [`logging.mdc`](rules/logging.mdc) - Logging and debugging standards
- [`security.mdc`](rules/security.mdc) - Security best practices and guidelines

## Rule Format

Each rule file follows the MDC (Markdown Configuration) format:

```yaml
---
description: "Rule description"
globs: ["file patterns"]
---

# Rule Content
```

### Common Structure

- Clear section headers
- YAML-formatted configurations
- Practical examples
- Best practices
- Common pitfalls to avoid
- Implementation guidelines

## Usage

1. **Rule Application**
   - Rules are automatically applied based on file patterns
   - Cursor AI uses these rules for suggestions and validations
   - Rules can be referenced in conversations using `@rule-name`

2. **Rule Precedence**

   ```yaml
   priority:
     1: Project-specific overrides
     2: Language/framework specific rules
     3: General best practices
   ```

3. **Rule Updates**
   - Rules are versioned with the project
   - Updates should be documented in commit messages
   - Breaking changes require major version bumps

## Integration with Cursor

These rules enhance Cursor's capabilities by:

- Providing consistent coding standards
- Automating documentation requirements
- Enforcing best practices
- Streamlining code reviews
- Maintaining security standards

## Contributing

To add or modify rules:

1. Follow the MDC format
2. Include clear examples
3. Document use cases
4. Test with Cursor AI
5. Submit a pull request

## Rule Validation

Rules are validated for:

- MDC format compliance
- YAML syntax
- Markdown structure
- Example completeness
- Documentation clarity

## Security Considerations

- Rules should not contain sensitive information
- Security-related rules must be reviewed by security team
- Credential patterns must be properly masked
- Access controls must be documented

## Support

For questions about these rules:

- Open an issue in the repository
- Contact the developer :)
- Check Cursor documentation
- Review existing rule implementations

## License

These rules are provided under the MIT License. See the LICENSE file in the root directory for details.
