# Development Conventions & Guidelines

## Table of Contents
1. [General Principles](#general-principles)
2. [Workflow](#workflow)
3. [Source Control](#source-control-git)
4. [Code Formatting](#code-formatting)
5. [Naming Conventions](#naming-conventions)
6. [Best Practices](#best-practices)


## General Principles
- Write clear and descriptive code.
- Prioritize readability over cleverness.
- Follow fundamental principles:
  - [SOLID](https://en.wikipedia.org/wiki/SOLID)
  - [SoC](https://en.wikipedia.org/wiki/Separation_of_concerns)
  - [KISS](https://en.wikipedia.org/wiki/KISS_principle)
  - [DRY](https://en.wikipedia.org/wiki/Don%27t_repeat_yourself)
  - [YAGNI](https://en.wikipedia.org/wiki/You_aren%27t_gonna_need_it)
  - [Fail Fast](https://en.wikipedia.org/wiki/Fail-fast_system)
- 


## Workflow
adopt "design first approach" [or waterfall](https://en.wikipedia.org/wiki/Waterfall_model)
- Before developing new feature - design it and document in confluence
- Each task starts as issue in Jira
- Task that requires changes in several repos should have child issue for each repo
- Feature that can't be deployed in one step (for example need preparation before and clean up after)
will have several issues, when first block latest
- Each issue will have feature branch named after issue in Jira
- 


## Source Control (Git)
- Check changes **before** commiting.
- Commit should follow push automatically (no local commits).
- Resolve merge conflict manually (you're always responsible of commit's content).
- Something went wrong when tried to resove conflict - better to stop, discard changes and start from scratch
- 


## Code Formatting
- Use prettier to format, with following configuration
{
  "printWidth": 120,
  "trailingComma": "es5",
  "tabWidth": 3,
  "semi": false,
  "singleQuote": true
}
- 


## Naming Conventions
- Use camelCase for variable names.
- Use PascalCase for class names.
- Use UPPER_CASE for global constants.
- Don't mix cases
- 


## Best Practices
- Write tests for all new features.
- Use await-async instead then-catch.
- Avoid long lines (over chaining) like complex ternaries, chaining of (await function) etc.
- Avoid oversized try-catch
- 

