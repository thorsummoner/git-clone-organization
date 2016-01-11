Git Clone Organization
======================

A _simple_ tool to clone all the repos in an organization. Works with 2-factor
auth by way of a [personal access token](https://github.com/settings/applications#personal-access-tokens).

### Usage

Download public org repos into a new/existing folder named after the org.
```
    ./git_clone_org <ORG_NAME>
```

Download public org repos into a new/existing folder specified; i.e current directory.
```
    ./git_clone_org <ORG_NAME> .
    ./git_clone_org <ORG_NAME> ./my_subfolder
    ./git_clone_org <ORG_NAME> /opt/abs_path
```

Declare the `--oauth` or `-a` flag with your Github Personal Access Token
to download private repositories.
```
    ./git_clone_org <ORG_NAME> --oauth=<OATH_TOKEN>
    ./git_clone_org <ORG_NAME> -a=<OATH_TOKEN>
```

### Installation

[Download](https://github.com/thorsummoner/git-clone-organization/releases) or Clone the `git_clone_org` program somewhere,
I recommend `/opt/git-clone-organization/` for unix-like systems.

Rename or link the program to your PATH under the name `git-clone-org`
for git-integration command structure; or call it directly as desired.


Usage With Git-Integration:
```
    git clone-org <ORG_NAME>
```

*Note: git-integration over-rides help documentation. To view help you must use the `-h` flag, not the `--help` flag.*
