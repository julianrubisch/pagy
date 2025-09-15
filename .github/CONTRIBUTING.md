# Pagy Contributions

> [!IMPORTANT]
> Pagy is imminently moving towards [v43](https://ddnexus.github.io/pagy-pre).
> - Please make PRs to the `master-pre` branch (v43) unless you are fixing a bug on the `master` branch.
> - If the changes are portable between `master-pre` and `master` it would be ideal if two PRs were submitted.
> - Please create a [version 43 discussion](https://github.com/ddnexus/pagy/discussions/new?category=version-43) before starting a PR in order to ensure your work will be included.

Pull Requests are welcome!

Here is a little useful information for contributing:

1. If you are planning for a complex PR, we suggest that you check beforehand whether your
   proposed changes are going to be accepted by posting your ideas in
   the [Feature Requests](https://github.com/ddnexus/pagy/discussions/categories/feature-requests) discussion area
2. For adding translations of locale dictionary files please follow
   the [locales  readme instructions here](https://github.com/ddnexus/pagy/blob/master/gem/locales/README.md).
3. **Pagy repo setup**
    - Clone pagy: `git clone https://github.com/ddnexus/pagy && cd pagy`
    - [Configure the git-hooks](https://github.com/ddnexus/pagy/tree/master/scripts/hooks)
4. **Development**
    - Please create your own branch out of `master` and use it for your development and PR
    - Ensure you are basing your PR on the `master` branch and keep rebasing it on `master` when it changes
    - **Code**
       - You can have a decent development environment already setup by just using one of the apps in
      the [Pagy Playground](https://ddnexus.github.io/pagy/playground) and/or
      with the [Pagy::Console](https://ddnexus.github.io/pagy/docs/api/console/) directly from the repo
    - **Docs**
      - The docs run on retype, and the repo is configured for its linux package. You may want to install the [platform specific npm package](https://retype.com/guides/getting-started/#platform-specific) in order to use it
      - `cd` in the pagy root directory
      - Install [bun](https://bun.sh/docs/installation)
      - Run `bun install`
      - Run `retype start`
      - Point your browser at `http://localhost:5000/pagy` for real-time feedback
5. **Testing**
    - If your PR **does not add any new feature** (e.g. a fix), please, just ensure that the "All checks have passed" indicator gets
      green light on the PR page (if it's not enabled, a maintainer will enable it for you)
    - If your PR **adds new features**, it needs [Ruby testing](https://github.com/ddnexus/pagy/tree/master/test) and/or
      [E2E testing](https://github.com/ddnexus/pagy/tree/master/e2e) or the coverage will fail. Ask for support if you need
      assistance.

Thank you!
