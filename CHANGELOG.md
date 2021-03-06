# Changelog

## 0.1.6

* Improvements
  * Add support for git tag and push.
    Use case is to tag a deployed version to a commit.
    Push pushes all new tags and commits to a given repository.
    (Thanks to @rohte)

## 0.1.5

* Improvements
  * Allow setting of a specific identity file (#12).
    Use case is to select the desired account from multiple GitHub accounts that have differing private repo membership.
    (Thanks to @markdingram)

## 0.1.4

* Bug Fixes:
  * Fixed bug in error handling in `wait-for-git` (#15)
    (Thanks to @ImmoStanke)

## 0.1.3

* Improvements
  * Allow specifying a timeout when cloning a repository

## 0.1.2

* Improvements
  * Made step-killing behavior of `wait-for-git` independent of polling frequency (#10)
  * Supporting known hosts files other than `~/.ssh/known_hosts` (e.g. `/etc/ssh/ssh_known_hosts`). (#9)
    Call `lambdacd-git.core/init-ssh!` instead of `lambdacd-git.ssh-agent-support/initialize-ssh-agent-support!` (which is now deprecated)
  * `lambdcd-git/ssh-agent-support/initialize-ssh-agent-support!` is deprecated and will be removed in subsequent releases.
    It is being replaced with `lambdacd-git.core/init-ssh!`

## 0.1.1

* Improvements
  * Added a way to notify `wait-for-git` through HTTP POST requests (#6)

## 0.1.0

* Initial Release 