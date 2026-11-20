# Contributing

Thanks for helping improve awesome-hacker-news!

## Adding or updating a project

[`src/sources.js`](src/sources.js) is the source of truth for the list and is also
published in the npm package. `README.md` is generated from it, so **don't edit the
README alone**: those changes will be overwritten the next time it is generated.

1. Add or update the project in the appropriate category in `src/sources.js`.
   Follow the format of the existing entries, including the project name, URL,
   and author details where available.
2. With Node.js and npm installed, regenerate the README from the repository root:

   ```sh
   npm run generate-md
   ```

   The generator sorts categories and projects alphabetically.
3. Review the generated `README.md` and include both `src/sources.js` and
   `README.md` in your pull request.

To change the README's introductory text or formatting, edit
[`src/generate-md.js`](src/generate-md.js) and run the same command rather than
editing the generated file directly.

## Pull request format

Every pull request must include all of these sections:

1. Screenshots: required for UI changes and visual fixes. Otherwise write `Not applicable: <reason>`.
2. Recordings: required for interaction changes, animations, and flows. Otherwise write `Not applicable: <reason>`.
3. What changed: a description in very simple language.
4. Before / After: what the function or behavior was before, and what it is now.
5. Alignment: why this task was chosen and prioritized over other work.

Keep any other required sections, such as Changelog (when this repo's changelog tooling reads `## Changelog`) and Testing.

Use `.github/pull_request_template.md` when opening a pull request. Do not merge a pull request that is missing any of these sections.

