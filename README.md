<p align="center">
  <a href="#">
    <img src="https://github.com/andry81-cache/andry81-devops--gh-content-cache/raw/master/repo/andry81-devops/gh-action--accum-content/badges/metrics/shields-repo-size.svg" valign="middle" alt="GitHub repo size in bytes" /></a>
<!-- -- >
• <a href="#">
    <img src="https://github.com/andry81-cache/andry81-devops--gh-content-cache/raw/master/repo/andry81-devops/gh-action--accum-content/badges/metrics/shields-code-size.svg" valign="middle" alt="code size in bytes" /></a>
<!-- -->
• <a href="https://github.com/XAMPPRocky/tokei">
    <img src="https://github.com/andry81-cache/andry81-devops--gh-content-cache/raw/master/repo/andry81-devops/gh-action--accum-content/badges/metrics/tokei-lines-of-code.svg" valign="middle" alt="lines of code by tokei.rs" /></a>
</p>

<p align="center">
  <a href="https://github.com/andry81-stats/gh-action--accum-content--gh-stats/commits/master/traffic/views">
    <img src="https://github.com/andry81-cache/andry81-devops--gh-content-cache/raw/master/repo/andry81-devops/gh-action--accum-content/badges/traffic/views/all.svg" valign="middle" alt="GitHub views|any|total" />
    <img src="https://github.com/andry81-cache/andry81-devops--gh-content-cache/raw/master/repo/andry81-devops/gh-action--accum-content/badges/traffic/views/all-14d.svg" valign="middle" alt="GitHub views|any|14d" /></a>
• <a href="https://github.com/andry81-stats/gh-action--accum-content--gh-stats/commits/master/traffic/views">
    <img src="https://github.com/andry81-cache/andry81-devops--gh-content-cache/raw/master/repo/andry81-devops/gh-action--accum-content/badges/traffic/views/unq.svg" valign="middle" alt="GitHub views|unique per day|total" />
    <img src="https://github.com/andry81-cache/andry81-devops--gh-content-cache/raw/master/repo/andry81-devops/gh-action--accum-content/badges/traffic/views/unq-14d.svg" valign="middle" alt="GitHub views|unique per day|14d" /></a>
</p>

<p align="center">
  <a href="https://github.com/andry81-stats/gh-action--accum-content--gh-stats/commits/master/traffic/clones">
    <img src="https://github.com/andry81-cache/andry81-devops--gh-content-cache/raw/master/repo/andry81-devops/gh-action--accum-content/badges/traffic/clones/all.svg" valign="middle" alt="GitHub clones|any|total" />
    <img src="https://github.com/andry81-cache/andry81-devops--gh-content-cache/raw/master/repo/andry81-devops/gh-action--accum-content/badges/traffic/clones/all-14d.svg" valign="middle" alt="GitHub clones|any|14d" /></a>
• <a href="https://github.com/andry81-stats/gh-action--accum-content--gh-stats/commits/master/traffic/clones">
    <img src="https://github.com/andry81-cache/andry81-devops--gh-content-cache/raw/master/repo/andry81-devops/gh-action--accum-content/badges/traffic/clones/unq.svg" valign="middle" alt="GitHub clones|unique per day|total" />
    <img src="https://github.com/andry81-cache/andry81-devops--gh-content-cache/raw/master/repo/andry81-devops/gh-action--accum-content/badges/traffic/clones/unq-14d.svg" valign="middle" alt="GitHub clones|unique per day|14d" /></a>
</p>

<p align="center">
  <a href="https://github.com/andry81-devops/gh-action--accum-content/commits">
    <img src="https://github.com/andry81-cache/andry81-devops--gh-content-cache/raw/master/repo/andry81-devops/gh-action--accum-content/badges/metrics/commits-since-latest.svg" valign="middle" alt="GitHub commits since latest version" /></a>
  <a href="https://github.com/andry81-devops/gh-action--accum-content/releases">
    <img src="https://github.com/andry81-cache/andry81-devops--gh-content-cache/raw/master/repo/andry81-devops/gh-action--accum-content/badges/metrics/latest-release-name.svg" valign="middle" alt="latest release name" /></a>
• <a href="https://github.com/andry81-devops/gh-action--accum-content/releases">
    <img src="https://github.com/andry81-cache/andry81-devops--gh-content-cache/raw/master/repo/andry81-devops/gh-action--accum-content/badges/metrics/github-all-releases.svg" valign="middle" alt="GitHub all releases" /></a>
</p>

<p align="center">
  <a href="https://github.com/andry81/donate"><img src="https://github.com/andry81-cache/gh-content-static-cache/raw/master/common/badges/donate/donate.svg" valign="middle" alt="donate" /></a>
</p>

---

<p align="center">
  <a href="https://github.com/andry81-devops/gh-action--accum-content/tree/HEAD/userlog.md">Userlog</a>
• <a href="https://github.com/andry81-devops/gh-action--accum-content/tree/HEAD/changelog.txt">Changelog</a>
• <a href="#dependecies">Dependencies</a>
• <a href="#known-issues">Known issues</a>
• <a href="#copyright-and-license"><img src="https://github.com/andry81-cache/gh-content-static-cache/raw/master/common/badges/license/mit-license.svg" valign="middle" alt="copyright and license" />&nbsp;Copyright and License</a>
</p>

<h4 align="center">GitHub composite action to periodically download and accumulate content into repository.<br />
<br />
Tutorial to use with: https://github.com/andry81-devops/accum-content</h4>

All tutorials: https://github.com/andry81/index#tutorials

##

# gh-action--accum-content@master

## Features:

* Does store downloaded content in a repository on the GitHub, so all the resources does render from a repository file and does access a repository instead of an external resource, and:

  * Prevents a broken link case holding at the same time the link content up to date and has option to roll back the content to previous version in case of broken or invalid content (if history was not rewrited and purged).

  * Reduces traffic to an external resource and avoids an out-of-service case.

  * Better does cacheing on the GitHub side, when a resource can be checked on a cache expiration and so updated opposite to an external resource, where the resource is relied on external caching and so has to be completely redownloaded.

* Content can be validated or/and altered after download, but before store in a repository. For example, for a SVG file - checks on valid values, size of canvas or malformed svg format.

* Downloads content under GitHub Actions pipeline IP instead of a client IP.

* Repository to store content config file and content itself can be different, and you may directly point the content repository as commits list:
  `https://github.com/{{REPO_OWNER}}/{{REPO}}--gh-content-cache/commits/{{BRANCH}}`

* Workflow is used [accum-content.sh](https://github.com/andry81-devops/gh-workflow/tree/HEAD/bash/cache/accum-content.sh) bash script to accumulate content

* The script does accumulate content into a repository and does update the content index file:
  `content-index.yml`

## Features of a standalone content cache repository:

* Can extract content not related to a specific repository or related to multiple repositories from a target repository.

* Can validate content by shell code handler before update it and filter out invalid content.

* Extracted content can be updated separately from a target repository. For example, after a release commit into a target repository.

* Traffic to an external resource can be replaced by traffic to the GitHub resource with better caching.

* All content can be stored in a single place and content change be saved into a commits list.

* Download and accumulate process can be controlled by explicit config file with parameters (can be outside of a content cache repository).

* The content cache repository can be rewrited to remove old files and history does not touching anything else.

## Functionality of the script:

* `CONTINUE_ON_INVALID_INPUT=1`, `CONTINUE_ON_EMPTY_CHANGES=1`:
  Treats invalid input or empty changes as not an error as by default.

* `ERROR_ON_EMPTY_CHANGES_WITHOUT_ERRORS=1` if `CONTINUE_ON_EMPTY_CHANGES=1`:
  Treats empty changes without errors as an error if enabled to continue on empty changes.

* `NO_SKIP_UNEXPIRED_ENTRIES=1`:
  Doesn't skip not yet expired entries and continue to process them.

* `NO_DOWNLOAD_ENTRIES=1`, `NO_DOWNLOAD_ENTRIES_AND_CREATE_EMPTY_INSTEAD=1`:
  Skips download of all entries to not wait on download at all.

* Uses and updates content index file `content-index.yml` to control the up to date and by default does generate the content index file from the content config file `content-config.yml`, if does not exist.

* `ENABLE_GENERATE_CHANGELOG_FILE=1`, `CHANGELOG_FILE=".../content-changelog.txt"`:
  Generates a textual changelog file with notes about changes per commit including the changes absence in case of skipped errors or skipped content update.

* `ENABLE_COMMIT_MESSAGE_DATE_WITH_TIME=1`:
  Inserts the time string in format `HH:MMZ` additionally after the date in each commit message (by default inserts only a date for shorter commit messages).

* `ENABLE_COMMIT_MESSAGE_WITH_WORKFLOW_RUN_NUMBER=1`:
  Inserts the workflow run number after date/time prefix in each commit message (by default does not insert for shorter commit messages).

* `ENABLE_GITHUB_ACTIONS_RUN_URL_PRINT_TO_CHANGELOG=1`:
  Prints GitHub Actions Run URL (with or without workflow run number) into the changelog file to reference the log on the GitHub from the changelog file.

* `ENABLE_REPO_STORE_COMMITS_URL_PRINT_TO_CHANGELOG=1`:
  Prints Content Store Repository commit URL into the changelog file to reference the commit from being committed changelog file.

  > **Note** The actual hash of the commit can not be know on the moment of the commit. So instead of the commit hash, an approximate date of the commit is used (~ +5 min ahead) in format of:
  > `https://github.com/{{REPO_OWNER}}/{{REPO}}--gh-content-cache/commits?branch={{BRANCH}}&time_zone=utc&until=YYYY-MM-DD`

* Can run download validation shell code after a file download (see `content-config.yml` example below).

* `USE_APT_GET_INSTALL_CMDLINE="<apt-get-install-cmdline>"`, `USE_PYTHON3_PIP_INSTALL_CMDLINE="<pip-install-cmdline>"`:
  Installs `apt-get` and `python3` packages and modules (w/o caching feature support) before script execution.

  > **Note** This is mostly for the testing purposes. In case of slow installation of many dependencies, packages or modules you have to use an installation together with the caching feature support.
  > See available list of solutions from here: https://stackoverflow.com/questions/59269850/caching-apt-packages-in-github-actions-workflow/73500415#73500415

# USAGE

> **Warning** You must replace all placeholder into respective values:

* `{{REPO_OWNER}}` -> repository owner
* `{{REPO}}` -> your repository
* `{{BRANCH}}` -> your repository branch or reference

## Examples:

<a name="content-config.yml">`{{REPO_OWNER}}/gh-content-cache-config/raw/master/repo/{{REPO_OWNER}}/{{REPO}}/content-config.yml`</a>:

```yml
content-config:

  entries:

    - init:
        #shell: bash
        ## Input variables:
        ##   GH_WORKFLOW_ROOT
        ##
        ## CAUTION:
        ##   First line must be a shebang line, otherwise each script line will run in a child bash process!
        ##
        #run: |
        #  #!/bin/bash
        #  exit 0

      dirs:

        - dir:            badges/traffic/views
          schedule:
            next-update:
              timestamp: 04:00Z

          #xpath-match-tokens: |
          #  svg/g[1]/text[3]

          files:

            - file:       all.svg
              query-url:  https://img.shields.io/badge/dynamic/json?color=success&label=views|all&query=count&url=https://github.com/andry81-stats/{{REPO}}--gh-stats/raw/master/traffic/views/latest-accum.json?raw=True&logo=github

            - file:       all-14d.svg
              query-url:  https://img.shields.io/badge/dynamic/json?color=success&label=14d&query=count&url=https://github.com/andry81-stats/{{REPO}}--gh-stats/raw/master/traffic/views/latest.json?raw=True

            - file:       unq.svg
              query-url:  https://img.shields.io/badge/dynamic/json?color=success&label=views|unq&query=uniques&url=https://github.com/andry81-stats/{{REPO}}--gh-stats/raw/master/traffic/views/latest-accum.json?raw=True&logo=github

            - file:       unq-14d.svg
              query-url:  https://img.shields.io/badge/dynamic/json?color=success&label=14d&query=uniques&url=https://github.com/andry81-stats/{{REPO}}--gh-stats/raw/master/traffic/views/latest.json?raw=True

        - dir:            badges/traffic/clones
          schedule:
            next-update:
              timestamp: 04:00Z

          #xpath-match-tokens: |
          #  svg/g[1]/text[3]

          files:

            - file:       all.svg
              query-url:  https://img.shields.io/badge/dynamic/json?color=success&label=clones|all&query=count&url=https://github.com/andry81-stats/{{REPO}}--gh-stats/raw/master/traffic/clones/latest-accum.json?raw=True&logo=github

            - file:       all-14d.svg
              query-url:  https://img.shields.io/badge/dynamic/json?color=success&label=14d&query=count&url=https://github.com/andry81-stats/{{REPO}}--gh-stats/raw/master/traffic/clones/latest.json?raw=True

            - file:       unq.svg
              query-url:  https://img.shields.io/badge/dynamic/json?color=success&label=clones|unq&query=uniques&url=https://github.com/andry81-stats/{{REPO}}--gh-stats/raw/master/traffic/clones/latest-accum.json?raw=True&logo=github

            - file:       unq-14d.svg
              query-url:  https://img.shields.io/badge/dynamic/json?color=success&label=14d&query=uniques&url=https://github.com/andry81-stats/{{REPO}}--gh-stats/raw/master/traffic/clones/latest.json?raw=True

        - dir:            badges/metrics
          schedule:
            next-update:
              timestamp: 08:00Z

          files:

            - file:       commits-since-latest.svg
              query-url:  https://img.shields.io/github/commits-since/{{REPO_OWNER}}/{{REPO}}/latest?sort=semver&label=Github%20commits%20since%20latest

            - file:       latest-release-name.svg
              query-url:  https://img.shields.io/github/v/release/{{REPO_OWNER}}/{{REPO}}?include_prereleases&label=latest

            - file:       github-all-releases.svg
              query-url:  https://img.shields.io/github/downloads/{{REPO_OWNER}}/{{REPO}}/total?label=Github%20dl|all&logo=github

        - dir:            badges/metrics
          schedule:
            next-update:
              timestamp: 08:00Z

          #xpath-match-tokens: |
          #  svg/g[1]/text[3]

          files:

            - file:       shields-repo-size.svg
              query-url:  https://img.shields.io/github/repo-size/{{REPO_OWNER}}/{{REPO}}?logo=github

            - file:       shields-code-size.svg
              query-url:  https://img.shields.io/github/languages/code-size/{{REPO_OWNER}}/{{REPO}}?logo=github

            - file:       tokei-lines-of-code.svg
              query-url:  https://tokei.rs/b1/github/{{REPO_OWNER}}/{{REPO}}?category=code

            #  download-validate:
            #    shell: bash
            #    # Input variables:
            #    #   GH_WORKFLOW_ROOT, GH_WORKFLOW_FLAGS,
            #    #   IS_STORED_FILE_EXIST, STORED_FILE, STORED_FILE_SIZE, STORED_FILE_HASH,
            #    #   DOWNLOADED_FILE, DOWNLOADED_FILE_SIZE, DOWNLOADED_FILE_HASH
            #    #
            #    # CAUTION:
            #    #   First line must be a shebang line, otherwise each script line will run in a child bash process!
            #    #
            #    run: |
            #      #!/bin/bash
            #      
            #      source "$GH_WORKFLOW_ROOT/_externals/tacklelib/bash/tacklelib/bash_tacklelib" || exit 255
            #      
            #      tkl_include_or_abort "$GH_WORKFLOW_ROOT/bash/github/init-xq-workflow.sh"
            #      
            #      if (( ${#XQ_CMDLINE_READ[@]} )); then
            #        IFS=$'\n' read -r value <<< "$("${XQ_CMDLINE_READ[@]}" '.svg.g[1].text[3]."#text"' "$DOWNLOADED_FILE")" || exit 255
            #      elif (( ${#XMLSTARLET_CMDLINE_SEL[@]} )); then
            #        value="$(sed 's/<svg [^>]*/<svg/' "$DOWNLOADED_FILE" | "${XMLSTARLET_CMDLINE_SEL[@]}" -t -v "//svg/g[2]/text[4]")" || exit 255
            #      else
            #        exit 255
            #      fi
            #      
            #      value="${value//[ $'\t'a-zA-Z]/}"
            #      value_int="${value%.*}"
            #      value_fract="${value#*.}"
            #      [[ "$value_fract" == "$value" ]] && value_fract=0
            #      (( value_int || value_fract )) && exit 0
            #      
            #      exit 255

            #- file:       tokei-lines.svg
            #  query-url:  https://img.shields.io/tokei/lines/github/{{REPO_OWNER}}/{{REPO}}?logo=tokei
```

<a name="accum-content-yml">`.github/workflows/accum-content.yml`</a>:

```yml
name: "content update at least every 3 hours"

on:
  schedule:
    - cron: "0 */3 * * *"
  # Allows you to run this workflow manually from the Actions tab
  workflow_dispatch:
    inputs:
      # for tests
      no_skip_unexpired_entries:
        description: 'Do not skip unexpired entries'
        required: false
        default: 'false'
      no_download_entries:
        description: 'Do not download entries'
        required: false
        default: 'false'

jobs:
  accum-content-cache:
    runs-on: ubuntu-latest

    steps:
      - uses: {{REPO_OWNER}}/gh-action--accum-content@master
        with:
          deps_repo_owner:          {{REPO_OWNER}}
          deps_repo_branch:         master
          deps_repo_read_token:     ${{ github.token }}

          config_repo_owner:        {{REPO_OWNER}}
          config_repo:              {{REPO}}--gh-content-cache-config
          config_repo_branch:       master
          config_repo_read_token:   ${{ secrets.READ_STATS_TOKEN }}

          store_repo_owner:         {{REPO_OWNER}}
          store_repo:               {{REPO}}--gh-content-cache
          store_repo_branch:        master
          store_repo_write_token:   ${{ secrets.READ_STATS_TOKEN }}

          commit_msg_entity:        my-store-dir-1

          # config repo
          content_config_file:      repo/{{REPO_OWNER}}/{{REPO}}/content-config.yml

          # store repo
          content_index_file:       repo/{{REPO_OWNER}}/{{REPO}}/content-index.yml

          content_index_dir:        repo/{{REPO_OWNER}}/{{REPO}}

          curl_flags: >-
            -H 'Cache-Control: no-cache'
            -v

          flags: >-
            ENABLE_PRINT_INITIAL_ENV_INTO_STDOUT=1

          env: >-
            ENABLE_GENERATE_CHANGELOG_FILE=1
            CHANGELOG_FILE=repo/{{REPO_OWNER}}/{{REPO}}/content-changelog.txt
            ENABLE_COMMIT_MESSAGE_DATE_WITH_TIME=1            # insert the time string in format HH:MMZ additionally after the date in each commit message
            ENABLE_COMMIT_MESSAGE_WITH_WORKFLOW_RUN_NUMBER=1  # insert the workflow run number after date/time prefix in each commit message
            ENABLE_YAML_DIFF_PRINT_AFTER_EDIT=1
            ENABLE_YAML_DIFF_PRINT_BEFORE_PATCH=1
            ENABLE_GITHUB_ACTIONS_RUN_URL_PRINT_TO_CHANGELOG=1
            ENABLE_REPO_STORE_COMMITS_URL_PRINT_TO_CHANGELOG=1
            CONTINUE_ON_EMPTY_CHANGES=1
            ERROR_ON_EMPTY_CHANGES_WITHOUT_ERRORS=1
          #  CONTINUE_ON_INVALID_INPUT=1
          #  ENABLE_YAML_PRINT_AFTER_EDIT=1
          #  ENABLE_YAML_PRINT_AFTER_PATCH=1
          #  ENABLE_YAML_PATCH_DIFF_PAUSE_MODE=1
          #  NO_SKIP_UNEXPIRED_ENTRIES=1
          #  NO_DOWNLOAD_ENTRIES=1
          #  NO_DOWNLOAD_ENTRIES_AND_CREATE_EMPTY_INSTEAD=1
          #  "USE_APT_GET_INSTALL_CMDLINE=-y xmlstarlet"
          #  "USE_PYTHON3_PIP_INSTALL_CMDLINE=xq"
```

> **Note** You can use `secrets.READ_STATS_TOKEN` instead of `secrets.WRITE_STATS_TOKEN` as long as both repositories under the same repository owner.

> **Warning** You must use different values for `deps_repo_owner`, `config_repo_owner` and `store_repo_owner` if respective repositories actually under different repository owners.

> **Note** See <a href="https://github.com/andry81-devops/github-accum-stats#reuse">REUSE</a> section for details if you have multiple repositories and want to store all GitHub workflow scripts (`.github/workflows/*.yml`) in a single repository.

## Dependencies

* https://github.com/andry81-devops/gh-workflow

## Known Issues

https://github.com/andry81-devops/gh-known-issues#known-issues

## Last known issues updates

https://github.com/andry81-devops/gh-known-issues#last-known-issues-updates

## Copyright and License

Code and documentation copyright 2022 Andrey Dibrov. Code released under [MIT License](https://github.com/andry81-devops/gh-action--accum-content/tree/HEAD/license.txt)
