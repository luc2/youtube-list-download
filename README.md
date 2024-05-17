youtube-list-download
=====================

Description
-----------

The objective of this project is to download YouTube videos from lists :

- Lists of URLs in text files
- YouTube playlists

Examples :

```
$ vim ~/.ytld/config.yml
$ ytld extract-from-text-files urls.txt plan.yml
$ ytld extract-from-text-files folder-containing-text-files plan.yml
$ ytld extract-personal-playlists plan.yml
$ vim plan.yml
$ ytld download plan.yml destination-folder
```

Development
-----------

### Cheat sheet

#### Start Go project

```
$ go mod init quoonel/youtube-list-download
```

#### Install cobra-cli

```
$ go install github.com/spf13/cobra-cli@latest
```

#### Generate Cobra files

```
$ vim ~/.cobra.yaml
```

```yaml
---
author: luc2 <luc2@users.noreply.github.com>
license: MIT
useViper: true
...
```

```
$ cobra-cli init
$ cobra-cli add extract-from-text-files
$ cobra-cli add extract-personal-playlists
$ cobra-cli add download
```

#### Download dependencies

```
$ go get
```
