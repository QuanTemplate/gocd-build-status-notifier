# gocd-build-status-notifier

See the old [readme](./og-README.md)

## development

- install `gradle` and run: 

```zsh
./gradlew build
```
- copy the `github-pr-status` jar from the `github-pr-status/build/libs` to the
`/srv/go-server/plugins/external`

## config

Make sure to use GH token instead of user & password for authentication

This could be configured through the UI in the `plugins` panel after clicking the gear icon or through `.github` file

```
oauth=<token of the CI bot>
```

`.github` file should be in the home folder of the `go` user in the `go-server`