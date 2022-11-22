# container-reports

This repo contains the output of [Syft](https://github.com/anchore/syft) and [Grype](https://github.com/anchore/grype) (and potentially other tools) scans of container images I share publicly.
These scans are ran as a part of the automated build process as seen in the respective images `.drone.yml`.

The output of these reports are first pushed to my internal git server ([Gitea](gitea.io)), which then syncs with Github
on a regular interval.

You can check the scan results of the current image you have pulled by running 
```console
$ echo $COMMIT
```
and finding the corresponding folder in this repo.