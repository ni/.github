
For NI employees, more details on using GitHub can be found [here](https://ni.visualstudio.com/DevCentral/_wiki/wikis/AppCentral.wiki/6072/GitHub), in Azure DevOps.

# Requirments for open source projects
You may use the repo [ni/Github-Repo-Template](https://github.com/ni/Github-Repo-Template) as a starting point or guide (do not use capital letters in your repo's name)

- LICENSE file in the root directory
- use the MIT license (approved by NI Legal for permissively open source projects). If you are considering copyleft (e.g. GPL), contact opensource@ni.com.
- LICENSE should include NI copyright at the top of the file
- CONTRIBUTING.md in the root directory that contains the Developer Certificate of Origin (DCO)
- .github/pull_request_template.md should include language that explicitly acknowledges the submission adheres to the DCO

For NI employees, you can read more about open source considerations in the [Open Source Handbook](https://ni.visualstudio.com/DevCentral/_wiki/wikis/AppCentral.wiki/20767/Open-Source-Handbook), in Azure DevOps.

# Repo configuration

## Initial setup
- repo name should be all lowercase with hyphens to separate words, e.g. `my-repo`
- README.md and CONTRIBUTING.md
- [CODEOWNERS](https://docs.github.com/en/repositories/managing-your-repositorys-settings-and-features/customizing-your-repository/about-code-owners) file specifying at least one owner for every file in the repo
- [.github/pull_request_template.md](https://docs.github.com/en/communities/using-templates-to-encourage-useful-issues-and-pull-requests/about-issue-and-pull-request-templates#pull-request-templates) file
- configure allowed merge types for pull requests (i.e. merge, squash, and/or rebase)
- enable [auto-merge](https://docs.github.com/en/pull-requests/collaborating-with-pull-requests/incorporating-changes-from-a-pull-request/automatically-merging-a-pull-request)
- configure one or more [issue templates](https://docs.github.com/en/communities/using-templates-to-encourage-useful-issues-and-pull-requests/configuring-issue-templates-for-your-repository). See ni/nimble for [examples](https://github.com/ni/nimble/blob/main/.github/ISSUE_TEMPLATE/bug_report.md)
- configure [GitHub Actions](https://docs.github.com/en/actions/quickstart) to run gating build(s) on PRs
 
## Branch naming
- default branch should be named `main`
- names should be in all lowercase, with hyphens to separate words, e.g. `my-feature-branch`
- user branches should be under a `users/<username>/` path
- collaborative feature branches should be under a `features/` path 

# Code review policy
- Reviewers should respond to code reviews within 24 hours of being added
  - A response can be a review comment, an approval/rejection, or even just a comment to the effect of "I'll look at this tomorrow"
