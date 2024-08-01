# <!-- <Repository name> -->

<!-- <About/description> -->

## Getting Started

<!-- ### Prerequisites -->

### Installation

- Clone this repo locally.

```sh
git clone <repository-url>
```

<!-- ### Usage -->

---

## Development

### Git Hooks

- Install [pre-commit](https://pre-commit.com/#install) on your system.

```sh
pip install pre-commit
```

- Install pre-commit hooks into your local repo clone.

```sh
pre-commit install
```

### Release Management

<!-- This repository does not follow a release branching strategy. -->
This repository follows a release branching strategy finishing with `release`.
<!-- This repository follows a release branching strategy starting with `release-candidate` and finishing with `release`. -->
<!-- This repository follows a release branching strategy starting with `release-beta`, progressing to `release-candidate`, and finishing with `release`. -->

This repository automatically creates releases from corresponding release branches. See [release_workflows.md](docs/release_workflows.md).

### Updating from the Template Repository

Fetch the latest changes from the `release` branch of the remote template repository, and then merge those changes into your current branch, allowing for unrelated histories.

```sh
git fetch https://github.com/NathanaelGandhi/template-repo release \
  && git merge FETCH_HEAD --allow-unrelated-histories
```

_If there are merge conflicts, resolve and add the changes, followed by ```git commit``` to continue with the merge._

---

## Code Owners

For details on code ownership and responsibilities, check out the [CODEOWNERS](docs/CODEOWNERS) file.

---

## License

For information about the project's licensing, please see the [LICENSE](LICENSE) file.

---

## Additional Documentation

For additional docs, check out the [docs](docs/) folder.
