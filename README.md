# Cursor Rules

A comprehensive collection of coding standards, best practices, and guidelines for modern TypeScript/React/Next.js applications.

## Overview

This repository contains a set of rules and guidelines for developing modern web applications using TypeScript, React 19, Next.js, and related technologies. These rules are designed to ensure code consistency, maintainability, and performance across projects.

### Problem Statement

Modern web development involves complex ecosystems with multiple technologies, frameworks, and patterns. Without clear guidelines, codebases can become inconsistent, difficult to maintain, and prone to performance issues.

### Solution

This collection of rules provides clear, actionable guidelines for developers to follow, ensuring consistent code quality, performance optimization, and adherence to best practices.

### Key Features

- Comprehensive coding standards for TypeScript and React
- Next.js specific guidelines for Server and Client Components
- Naming conventions for files, folders, and code elements
- Performance optimization strategies
- UI and styling standards using Shadcn UI and Tailwind CSS
- Database querying patterns with Drizzle

### Technologies Covered

- TypeScript
- React 19
- Next.js 13+
- Tailwind CSS V4
- Shadcn UI
- Drizzle ORM

## Rules Overview

### Core Development Principles

- **000-agent.mdc**: Overall coding style and principles
- **110-styles.mdc**: General code style guidelines

### Naming and Structure

- **100-naming-conventions.mdc**: Consistent naming for files, folders, and code elements

### React and Next.js

- **101-client-components.mdc**: Guidelines for React Client Components
- **102-create-components.mdc**: Component creation standards
- **104-nextjs-backend.mdc**: Next.js backend implementation
- **105-nextjs-routes.mdc**: Next.js routing standards
- **107-server-components.mdc**: Guidelines for React Server Components
- **109-streaming-components.mdc**: Streaming component implementation

### UI and Styling

- **108-shadcn-ui.mdc**: Shadcn UI implementation guidelines
- **111-tailwind-styles.mdc**: Tailwind CSS v4 usage standards

### Database

- **106-postgres.mdc**: PostgreSQL and database standards

### Documentation

- **103-readme.mdc**: README standards for project documentation

### Refactoring

- **300-refactor-ref-react-19.mdc**: Guidelines for refactoring to React 19

## Usage

### Integration with Your Project

These rules are designed to be used with the Cursor editor or similar tools that can enforce coding standards. To use these rules:

1. Clone this repository or copy the rules into your project's `.cursor/rules/` directory
2. Configure your editor to recognize and enforce these rules
3. Share the rules with your team to ensure consistent coding practices

### Rule Format

Each rule file follows a standard format:

```
---
description: Brief description of the rule's purpose
globs: File patterns where this rule applies
---

## Context
Explanation of when and why to apply this rule

## Requirements
Detailed guidelines and requirements

## Examples
Code examples showing correct and incorrect usage
```

## Key Conventions

### TypeScript Usage

- Use TypeScript for all code
- Prefer types over interfaces
- Avoid enums; use maps instead
- Use functional components with TypeScript types

### React Patterns

- Minimize `use client`, `useEffect`, and `setState`
- Favor React Server Components (RSC) when possible
- Wrap client components in `Suspense` with fallback
- Use dynamic loading for non-critical components

### Styling

- Use Shadcn UI, Radix, and Tailwind for components and styling
- Implement responsive design with Tailwind CSS using a mobile-first approach
- Follow specific Tailwind best practices (e.g., prefer `flex gap-n` over `space-y-n`)

### Performance

- Optimize Web Vitals (LCP, CLS, FID)
- Use 'nuqs' for URL search parameter state management
- Optimize images: use WebP format, include size data, and implement lazy loading

## Contributing

Contributions to improve or extend these rules are welcome. Please follow these steps:

1. Fork the repository
2. Create a feature branch
3. Add or modify rules
4. Submit a pull request with a clear description of changes

## License

This project is licensed under the MIT License - see the [LICENSE.md](LICENSE.md) file for details.
