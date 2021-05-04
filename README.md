# semver-release
This repo use github branch name to release semver

<h3 align="center">Semver Release</h3>
<p align="center">This is an action release a version based on your branch name<p>

## Usage

This GitHub Action pins an issue based on a specified label. 


## Setup

```yaml
# .github/workflows/take.yml 
name: Assign issue to contributor
on: 
  issue_comment:

jobs:
  assign:
    name: Take an issue
    runs-on: ubuntu-latest
    steps:
    - name: take the issue
      uses: Shobhit05/semver-release-branch@main
      env:
        GITHUB_TOKEN: ${{ github.token }}
```
