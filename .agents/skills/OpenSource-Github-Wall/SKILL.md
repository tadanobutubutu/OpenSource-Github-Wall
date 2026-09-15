```markdown
# OpenSource-Github-Wall Development Patterns

> Auto-generated skill from repository analysis

## Overview
This skill teaches you the core development patterns and workflows of the OpenSource-Github-Wall repository, a TypeScript project that manages contributor profiles and displays them in a visual grid. You'll learn about the repository's coding conventions, how to add and merge contributor profiles, update the contributor grid, and follow best practices for contributing and testing.

## Coding Conventions

- **Language:** TypeScript
- **Framework:** None detected
- **File Naming:** PascalCase is used for file names.
  - Example: `ContributorProfile.ts`
- **Import Style:** Relative imports are preferred.
  - Example:
    ```typescript
    import { Contributor } from './Contributor';
    ```
- **Export Style:** Named exports are used.
  - Example:
    ```typescript
    export function getContributors() { ... }
    export const CONTRIBUTOR_LIMIT = 100;
    ```
- **Commit Messages:** Freeform, average length ~34 characters.

## Workflows

### Add Contributor Profile
**Trigger:** When you want to add yourself as a contributor to the Open Github Wall.  
**Command:** `/add-contributor`

1. Create a new JSON file in the `contributors/` directory. Name the file after your GitHub username (e.g., `contributors/janedoe.json`).
2. Fill in your contributor profile details in the JSON file.
   ```json
   {
     "name": "Jane Doe",
     "github": "janedoe",
     "bio": "Open source enthusiast."
   }
   ```
3. Commit the new JSON file with a message like:  
   `Add janedoe to contributors`
4. Optionally, open a pull request for your addition.

### Merge Contributor Profile PR
**Trigger:** When a contributor submits a pull request to add their profile.  
**Command:** `/merge-contributor-pr`

1. Review the pull request containing the new `contributors/*.json` file.
2. Ensure the JSON file is valid and follows the expected structure.
3. Merge the pull request into the main branch.

### Update Contributor Grid
**Trigger:** When new contributors are added or the contributor list needs to be updated.  
**Command:** `/update-contributor-grid`

1. Edit `README.md` to refresh the visual grid or list of contributors.
2. Add new contributors or update the display as needed.
3. Commit the changes with a message like:  
   `Update contributor grid in README.md`

## Testing Patterns

- **Framework:** Unknown (not detected)
- **Test File Pattern:** Test files follow the `*.test.*` naming convention.
  - Example: `Contributor.test.ts`
- **Test Structure:** (Assumed) Standard TypeScript test structure, e.g.:
  ```typescript
  import { getContributors } from './Contributor';

  test('should return all contributors', () => {
    const contributors = getContributors();
    expect(contributors.length).toBeGreaterThan(0);
  });
  ```

## Commands

| Command                  | Purpose                                                         |
|--------------------------|-----------------------------------------------------------------|
| /add-contributor         | Add a new contributor profile to the project                    |
| /merge-contributor-pr    | Merge a pull request that adds a new contributor profile        |
| /update-contributor-grid | Update the README.md contributor grid or list                   |
```
