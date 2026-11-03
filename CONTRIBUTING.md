# CONTRIBUTING

## Requirements

- Changes should be related to project
- Changes should be verified
- Changes should not violate license of any of items
- All commits must be signed (see [Signed commits](#signed-commits))

## Signed commits

For safety reasons, every commit in a PR must be **signed** and shown as
**Verified** on GitHub. PRs that contain unsigned or unverified commits fail the
`Signed Commits` check and will not be merged.

You can sign commits with GPG, SSH or S/MIME. For example, with an SSH key:

```sh
git config --global gpg.format ssh
git config --global user.signingkey ~/.ssh/id_ed25519.pub
git config --global commit.gpgsign true
```

Then add the same key to your GitHub account as a **Signing Key**
(Settings → SSH and GPG keys). The commit email must match a verified email of
your GitHub account.

To sign commits you already pushed, re-sign them and force-push your branch:

```sh
git rebase --exec 'git commit --amend --no-edit -S' origin/master
git push --force-with-lease
```

See the GitHub docs: [About commit signature verification](https://docs.github.com/en/authentication/managing-commit-signature-verification/about-commit-signature-verification).

## Minimum requirements for new entries

The same rules apply to every link you add, in any section, list, table or
Resources:

- A GitHub repository is good to have, but not required
- If the link has a GitHub repository, it must be more than 45 days old
- If the link has a GitHub repository, it must have more than 30 stars

"Age" is the age of the **project's GitHub repository**, counted from its
creation date. It is not the age of your account. If your project does not meet
these rules yet, feel free to open a PR again once it does.

Separately from the project rules above:

- Your own GitHub account must be older than 180 days
- Disclose in the PR body if you are the author or maintainer of the project
- Do not submit the same project to this list more than once
- PRs from new accounts or accounts that send the same submission to many lists
  may be closed automatically by the PR Spam Guard

## Discussing on PR or Issue

- Please read `CODE_OF_CONDUCT.md`

## Thank you for your contribution
