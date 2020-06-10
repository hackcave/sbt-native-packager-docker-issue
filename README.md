# sbt-native-packager-docker-issue-1304

Original bug report at [https://github.com/sbt/sbt-native-packager/issues/1304](https://github.com/sbt/sbt-native-packager/issues/1304)

To reproduce the bug:

```bash
git clone https://github.com/hackcave/sbt-native-packager-docker-issue.git
cd sbt-native-packager-docker-issue && sbt docker:publishLocal
```

It fails with this error:
```
chmod: cannot access 'opt/bin/docker/entrypoint.sh': No such file or directory
The command 'chmod u+x,g+x opt/bin/docker/entrypoint.sh' returned a non-zero code: 1
```
