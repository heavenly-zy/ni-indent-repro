Requires Node.js >= 20.19 and pnpm 12.5.1.

**Before running the commands, make sure the root `package.json` uses CRLF line endings. If it uses LF, change it to CRLF in your editor and save the file.**

Run the following commands from the project root:

```sh
pnpm install
pnpm exec ni -D is-number
```

Expected: `"is-number": "catalog:"` is added to `devDependencies` without introducing extra blank lines.

Actual: The package is installed successfully, but extra blank lines appear in `package.json`.
