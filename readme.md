## cheetah for cloudflare workers

### File Structure

- `.github`
  - `workflows`
    - `bump.yml` *- updates your dependencies daily at 2pm* **(make sure to update the `reviewers` property!)**
- `.vscode`
  - `settings.json` *- enables deno for this workspace*
- `.gitignore`
- `deno.json` *- for managing tasks and dependencies*
- `mod.ts` *- the entry file for your app*
- `wrangler.toml` *- for managing your worker*

### Get Started

1. Make sure to replace the `name`, `account_id`, and `route` in the `wrangler.toml` file.

2. Don't forget to replace `YOUR_GITHUB_USERNAME` with your username in the `.github/workflows/bump.yml` file. You can learn more [here](https://github.com/azurystudio/bump#readme).

3. If you want to transpile your app into a single JavaScript file, run `deno task build` in your terminal.

4. To publish it, simply run `deno task publish`.
