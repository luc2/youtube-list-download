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

#### Starting a new project

```
$ go mod init quoonel/youtube-list-download
$ go get
```
