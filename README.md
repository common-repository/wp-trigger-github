# wp-trigger-github

Plugin for WordPress.
Save or update action triggers Github repository_dispatch action for triggering Github Actions workflow.

## Installation

- Add to WordPress and activate
- Go to Settings -> General and scroll to bottom
- Add repository owner name, repository name and generated personal access token
- If you want to see status badge on dashboard, add workflow name too.

## GitHub Actions configuration

In your GitHub workflow yaml file, you can use this as:

```yml
on:
  repository_dispatch:
    types: [wordpress]
```

or if you don't want to specify type you can use it without `types`

```yml
on:
  repository_dispatch:
```
