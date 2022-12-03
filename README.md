# GitHub Action: Delete tag and release

[![main](https://github.com/unkies/action-gh-delete-release/actions/workflows/main.yaml/badge.svg?branch=master)](https://github.com/unkies/action-gh-delete-release/actions/workflows/main.yaml)

Add following step to your workflow:

```yaml
- uses: unkies/delete-tag-and-release@v0.2.1
  with:
    delete_release: true # default: false
    tag_name: v0.1.0 # tag name to delete
    repo: <owner>/<repoName> # target repo (optional). defaults to repo running this action
  env:
    GITHUB_TOKEN: ${{ secrets.GITHUB_TOKEN }}
```

## History

This project was taken from [here](https://github.com/dev-drprasad/delete-tag-and-release).