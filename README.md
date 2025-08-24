# Shared Utilities Library

A collection of common utilities and helper functions used across multiple services in our organization.

## Overview

This library provides reusable components, utilities, and helper functions that are shared across our microservices architecture, including user-service, payment-service, frontend-web, and mobile-app.

## Features

- **Validation Utilities**: Email, phone, and data validation helpers
- **Date & Time Helpers**: Formatting, timezone conversion, date calculations
- **String Utilities**: Sanitization, formatting, and manipulation functions
- **API Helpers**: HTTP client wrappers, response formatting
- **Logging Utilities**: Structured logging with different levels
- **Error Handling**: Standardized error types and handling
- **Configuration Management**: Environment-based config loading

## Installation

```bash
npm install @yourorg/shared-utilities-lib
```

## Quick Start

```javascript
import { validateEmail, formatDate, apiClient } from '@yourorg/shared-utilities-lib';

// Email validation
const isValid = validateEmail('user@example.com');

// Date formatting
const formatted = formatDate(new Date(), 'YYYY-MM-DD');

// API calls with built-in error handling
const response = await apiClient.get('/api/users');
```

## Testing

We maintain >90% test coverage with comprehensive unit tests for all utility functions.

## CI/CD Pipeline

### GitHub Actions Workflows

- **Test**: Runs on all PRs and pushes
- **Build**: Validates build process
- **Security**: Dependency vulnerability scanning
- **Release**: Automated publishing to npm

### Quality Gates

- ✅ All tests must pass
- ✅ Code coverage >90%
- ✅ No ESLint errors
- ✅ No security vulnerabilities
- ✅ TypeScript compilation successful

## Contributing

1. Create feature branch from `main`
2. Write code with comprehensive tests
3. Update documentation
4. Ensure all CI checks pass
5. Request review from core team

## Versioning & Releases

We follow [Semantic Versioning](https://semver.org/):
- **MAJOR**: Breaking changes
- **MINOR**: New features (backward compatible)
- **PATCH**: Bug fixes (backward compatible)

Current version: **2.1.4**

## Support & Contact

- **Issues**: Create GitHub issue with detailed description
- **Slack**: #shared-utilities-support
- **Email**: platform-team@yourorg.com

## License

MIT License - see LICENSE file for details
