# ESR: Firefox 45.2.0esr

### Started: 16-06-02

## Build 1

### ESR Graph 1
[task graph](https://tools.taskcluster.net/task-group-inspector/#HPwlXKDcRdemzxRNOz11Iw)

#### Status
- [x] [submit to Shipit](https://wiki.mozilla.org/Release:Release_Automation_on_Mercurial:Starting_a_Release#Submit_to_Ship_It)

### ESR Graph 2
task graph url: unknown

#### Status
- [ ] [pushed to mirrors/releases](../how-tos/relpro.md#2-push-to-releases-dir-mirrors)
- [ ] [publish in Balrog](../how-tos/relpro.md#3-publish-in-balrog)
- [ ] [post-release tasks](../how-tos/relpro.md#4-post-release-step)

### Issues
- Old release process started in parallel with release promotion, because bm81's release-runner was out of date and grabbed the release at the same time with relpro. Updated the checkout, restarted release-runner. Stopped running builds
- The old process bumped the version on default, what caused some l10n repacks to rerun. Filed bug 1277443 to address the issue.
- aW9wfgRNRXSDOxvko0x6aQ firefox mozilla-esr45 win32 l10n repack 6/10 timed out. Manually reran using tctalker

