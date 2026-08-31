```markdown
# huashu-design Development Patterns

> Auto-generated skill from repository analysis

## Overview
This skill teaches the core development patterns and workflows used in the `huashu-design` TypeScript codebase. It covers file naming conventions, import/export styles, commit practices, and step-by-step guides for common repository workflows such as fixing demo assets and updating scripts with documentation.

## Coding Conventions

- **File Naming:**  
  Use **kebab-case** for all file names.  
  _Example:_  
  ```
  my-component.ts
  demo-page.test.ts
  ```

- **Import Style:**  
  Use **relative imports** for referencing modules within the project.  
  _Example:_  
  ```typescript
  import { MyComponent } from './my-component';
  ```

- **Export Style:**  
  Use **named exports** instead of default exports.  
  _Example:_  
  ```typescript
  // my-component.ts
  export function MyComponent() { /* ... */ }

  // usage
  import { MyComponent } from './my-component';
  ```

- **Commit Messages:**  
  - Prefix with `fix` or `feat` as appropriate.
  - Keep messages concise (~51 characters on average).
  _Example:_  
  ```
  fix: restore missing image in demo page
  feat: add new button component
  ```

## Workflows

### Bugfix Demo HTML Assets
**Trigger:** When a demo page needs to be fixed due to missing assets or display issues  
**Command:** `/fix-demo-asset`

1. Identify the broken or missing asset in `demos/*.html`.
2. Update or restore the relevant demo HTML files.
3. Commit the changes with a `fix` message referencing the demo and issue.

_Example commit message:_  
```
fix: restore missing logo in demos/button-demo.html
```

### Update Script and Reference Doc
**Trigger:** When a script is upgraded or its usage changes, requiring both code and documentation updates  
**Command:** `/update-script-doc`

1. Modify the script file in `scripts/*.mjs` to implement the new logic or API.
   ```typescript
   // scripts/example.mjs
   export function updatedFeature() { /* new logic */ }
   ```
2. Update the related documentation in `references/*.md` to describe the new behavior.
   ```
   ## updatedFeature
   This function now accepts an options object for configuration.
   ```
3. Commit both files together with a descriptive message.
   ```
   feat: update example.mjs and docs for new options API
   ```

## Testing Patterns

- **Test File Pattern:**  
  Test files follow the `*.test.*` naming convention.  
  _Example:_  
  ```
  my-component.test.ts
  ```
- **Testing Framework:**  
  Not explicitly detected; follow the file pattern for placement.

- **Test Example:**  
  ```typescript
  // my-component.test.ts
  import { MyComponent } from './my-component';

  describe('MyComponent', () => {
    it('should render correctly', () => {
      // test implementation
    });
  });
  ```

## Commands

| Command            | Purpose                                                        |
|--------------------|----------------------------------------------------------------|
| /fix-demo-asset    | Restore or update demo HTML files with missing or broken assets|
| /update-script-doc | Update a script and its corresponding documentation            |
```
