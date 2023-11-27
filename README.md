# Npm Package Examples

Monorepo for different example npm packages.

## Publishing

- `npm publish --workspaces --access public` to publish all workspaces manually.
- Create a new release on GitHub to publish all workspaces to Github Packages.

  - Publish the release to publish all workspaces to npm.
  - To use the packages from GitHub Packages, you need to add a `.npmrc` file to your project root with the following content:

    ```text
    @fukaraadam-workspace:registry=https://npm.pkg.github.com
    ```

    Then, you can install the packages with `npm install @fukaraadam-workspace/<package-name>`.
