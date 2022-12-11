> :information_source: this log lists user most visible changes

> :warning: to find all changes use [changelog.txt](https://github.com/andry81-devops/gh-action--accum-content/blob/master/changelog.txt) file in a directory

## 2022.12.11:
* new: action.yml: added `ENABLE_COMMIT_REFERENCE_URL_PRINT_TO_CHANGELOG` variable to be able to print Commit Reference URL into the changelog file

## 2022.10.12:
* new: action.yml: added `flags` parameter with builtin parse into `GH_WORKFLOW_FLAGS` environment variable as a single line string
* new: action.yml: added ability to insert workflow run number into commit message after date/time prefix (`ENABLE_COMMIT_MESSAGE_WITH_WORKFLOW_RUN_NUMBER=1`)
* changed: action.yml: use `$GH_WORKFLOW_ROOT/_common/update-permissions.sh` script to automate permissions update

## 2022.09.08:
* fixed: action.yml: multiline input in `${{ input.env }}`

## 2022.09.01:
* new: action.yml: install `xmlstarlet` package into `ubuntu-latest` using `awalsh128/cache-apt-pkgs-action` as forked repo

## 2022.08.29:
* new: action.yml: added `USE_PYTHON3_PIP_INSTALL_CMDLINE` and `USE_APT_GET_INSTALL_CMDLINE` variable to install python3 and apt-get prerequisites
* new: action.yml: added `NO_DOWNLOAD_ENTRIES` environment variable and check for `no_download_entries` of workflow dispatch input parameter to avoid entries download

## 2022.08.26:
* new: action.yml: added `ENABLE_GITHUB_ACTIONS_RUN_URL_PRINT_TO_CHANGELOG` and `GHWF_GITHUB_ACTIONS_RUN_URL` variables to be able to print GitHub Actions run URL into the changelog file

## 2022.08.12:
* new: action.yml: flush print annotations at the last always executed step

## 2022.08.09:
* new: action.yml: print commit reference url to the log

## 2022.06.03:
* fixed: action.yml: `content changelog file` invalid path notice

## 2022.05.12:
* new: action.yml: added `NO_SKIP_UNEXPIRED_ENTRIES` environment variable and check for `no_skip_unexpired_entries` of workflow dispatch input parameter to avoid skip of unexpired entries

## 2022.05.11:
* new: action.yml: added `commit_msg_entity` optional input parameter as replacement of `stat_entity` in the commit message
* changed: action.yml: removed `store_entity_path` input parameter
* changed: action.yml: swapped `COMMIT_MESSAGE_PREFIX` and `COMMIT_MESSAGE_SUFFIX` in all scripts to further improve readability in case of GitHub commit message truncation

## 2022.05.06:
* fixed: action.yml: `CHANGELOG_FILE` must be always not empty

## 2022.05.04:
* new: action.yml: added `COMMIT_MESSAGE_PREFIX` to split an automated user commit message into prefix and suffix parts

## 2022.04.30:
* changed: action.yml: implementation is reworked

## 2022.04.16:
* fixed: action.yml: `mkdir` in a working copy moved after git checkout instead of before to avoid accidental remove on cleanup
* changed: action.yml: added `mkdir-p` parameter usage

## 2022.04.15:
* changed: action.yml: switched to use `andry81-devops/gh-action--git-checkout` action instead of `actions/checkout`
