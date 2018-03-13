# chen-shy.github.io

## start

```
$ bundle install
$ rake watch # for development
$ rake build # for building (and deployment)
```

## create new project for XXX

- create new org XXX

### `attachments` repo

- create attachments repo under XXX org
- enable Github Pages
- upload photos
- get link like https://XXX.github.io/attachments/69.jpg for main photo

### `XXX.github.io` repo

- fork ann-dau.github.io repo to XXX org
- rename to XXX.github.io
- grant travis-ci to access the new repo https://github.com/settings/connections/applications/f244293c729d5066cf27
- sync account https://travis-ci.org/profile/wxxeibo and repload page
- enable XXX/XXX.github.io
- enable `Build only if .travis.yml is present`
- go to setting, add `PASSWORD` in env vars
- `bundle install` in project dir
- `rake watch` to start dev server
- change ann-dau in source code to XXX, and commit
- restart `rake watch` for changing of `_config_localhost.yml`
- commit

### google search console

https://www.google.com/webmasters/tools/submit-url

### google analytics

- create new website
- update tracking code in `_config.yml`
- commit

## add new photos

1. add new photos to attachments repo
1. push commit
1. run gen.sh in xxx.github.io repo
1. push commit