# Beta: Firefox 50.0b6

### Started: 2016-10-10

## Build 1

### Beta Graph
[task group](https://tools.taskcluster.net/push-inspector/#/ab1WuG6YSvSXJNEx95fakw)


#### Status
- [x] [submit to Shipit](https://wiki.mozilla.org/Release:Release_Automation_on_Mercurial:Starting_a_Release#Submit_to_Ship_It)
- [x] [emailed beta-cdntest](../how-tos/relpro.md#1-email-drivers-re-release-live-on-test-channel)
- [x] [published release tasks](../how-tos/relpro.md#3-publish-release)

### Issues
- [Bug 1307326](https://bugzil.la/1307326): linux-opt TC tier-2 task finished earlier that BB linux-opt
- [Bug 1309252](https://bugzil.la/1309252): lij mac dmg was uploaded corrupted by beetmover. Need to rerun the corresponding beetmover task and regenerate the checksums after the purge. It turned out that the file was badly cached in TC cloud-mirror. Rail had to use a one-click-loaner to be able to get the cloud-mirror URLs. He replaced `/redirect/` in the URL to `/purge/` and used `curl -X DELETE` to purge the bad file from the cache. Followed https://gist.github.com/rail/7e59d6756b9611c379c0523660eab6d8 for the rest
- [Bug 1309348](https://bugzil.la/1309348): to handle beetmover issues in the future


