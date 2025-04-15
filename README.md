# GitHub Actions 実験室

## `GitHub Actions`を導入するためのルール

下記フォルダ、ファイル名で`YAML`ファイルを保存する

```
.github\workflows\github-actions-ci.yml
```

github-actions-ci.yml

```yaml
name: GitHub Actions CI
on: push
jobs:
  GitHub-Actions-CI:
    runs-on: ubuntu-latest
    steps:
      - uses: actions/checkout@v4
      - run: echo "Hello, GitHub Actions"
```
