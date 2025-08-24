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
```

// API calls with built-in error handling
const response = await apiClient.get('/api/users');
