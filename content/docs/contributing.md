+++
title = 'Contributing'
date = '2025-09-26T21:03:00+10:00'
draft = false
+++

{{< callout type="warning" >}}
Uploading entire breach dumps is **not** allowed. Only include password lists that do not contain any personally identifiable information.
{{< /callout >}}

## How to contribute

- Open a pull request with your wordlists or documentation changes.
- Or create an issue that links to the material you would like to include.

Always credit original authors and sources whenever possible.

## Folder naming

Use train case for directories, for example `File-System`.

## README entries

When adding a new wordlist:

1. Add an entry to the containing folder's `README.md`. Create the README if it does not exist.
2. Use the filename as the heading so readers can match entries quickly.
3. Add a `Use for:` note if the wordlist targets a specific scenario.
4. Include `Source:` and (if available) `Reference:` links to the author or related write-up.

See the [`Discovery/Web-Content`](https://github.com/danielmiessler/SecLists/tree/master/Discovery/Web-Content) README for formatting inspiration.

## Conventional commits (optional)

SecLists encourages the [Conventional Commits](https://www.conventionalcommits.org/en/v1.0.0/) style. Examples:

```
feat(wordlist): add "raft" wordlists by Google
fix(docs): correct author name for raft.txt entry
chore(wordlist): move file extension lists to /Fuzzing/File-Extensions/
```

Use the commit type that best describes the change (wordlist, docs, cicd, etc.).
