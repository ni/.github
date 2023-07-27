For NI employees, more details on using GitHub can be found [here](https://ni.visualstudio.com/DevCentral/_wiki/wikis/AppCentral.wiki/6072/GitHub), in Azure DevOps.

# Requirements for open source projects

You may use the repo [ni/Github-Repo-Template](https://github.com/ni/Github-Repo-Template) as a starting point or guide (do not use capital letters in your repo's name)

- Include a LICENSE file in the root directory
    - Use the MIT license (approved by NI Legal for permissively open source projects). If you are considering copyleft (e.g. GPL), contact opensource@ni.com.
    - LICENSE should include NI copyright at the top of the file (e.g. "Copyright (c) 2022, National Instruments Corp.")
- Include a CONTRIBUTING.md in the root directory
    - It should contain the [Developer Certificate of Origin (DCO)](https://developercertificate.org/)
- Install the [GitHub DCO App](https://github.com/apps/dco) for this repository to ensure DCO compliance by all contributors.

For NI employees, you can read more about open source considerations in the [Open Source Handbook](https://ni.visualstudio.com/DevCentral/_wiki/wikis/AppCentral.wiki/20767/Open-Source-Handbook), in Azure DevOps.

# Repo configuration

## Initial setup

- Repo name should be all lowercase with hyphens to separate words, e.g. `my-repo`
- Include helpful README.md and CONTRIBUTING.md
- Include a [CODEOWNERS](https://docs.github.com/en/repositories/managing-your-repositorys-settings-and-features/customizing-your-repository/about-code-owners) file specifying at least one owner for every file in the repo
- Include a [.github/pull_request_template.md](https://docs.github.com/en/communities/using-templates-to-encourage-useful-issues-and-pull-requests/about-issue-and-pull-request-templates#pull-request-templates) file
- Configure allowed merge types for pull requests (i.e. merge, squash, and/or rebase)
- Enable [auto-merge](https://docs.github.com/en/pull-requests/collaborating-with-pull-requests/incorporating-changes-from-a-pull-request/automatically-merging-a-pull-request)
- Configure one or more [issue templates](https://docs.github.com/en/communities/using-templates-to-encourage-useful-issues-and-pull-requests/configuring-issue-templates-for-your-repository). See ni/nimble for [examples](https://github.com/ni/nimble/blob/main/.github/ISSUE_TEMPLATE/bug_report.md)
- Configure [GitHub Actions](https://docs.github.com/en/actions/quickstart) to run gating build(s) on PRs. You can also use Azure Pipelines if the build requires access to NI build agents.
 
## Branch naming

- Default branch should be named `main`
- Names should be in all lowercase, with hyphens to separate words, e.g. `my-feature-branch`
- User branches should be under `users/<username>/`
- Collaborative feature branches should be under `features/`

# Code review policy

- Reviewers should respond to code reviews within 24 hours of being added (minus weekends and holidays)
  - A response can be a review comment, an approval/rejection, or even just a comment to the effect of "I'll look at this tomorrow"
