# Shiori

Shiori is a simple bookmarks manager written in the Go language. Intended as a simple clone of Pocket. You can use it as a command line application or as a web application. This application is distributed as a single binary, which means it can be installed and used easily.

github.com/go-shiori/shiori

<img src="https://raw.githubusercontent.com/go-shiori/shiori/refs/heads/master/docs/assets/logos/shiori-logo-1024.png" width="60%" height="auto" alt="shiori logo">

## How to use this Makejail

```sh
appjail makejail \
    -j shiori \
    -f gh+AppJail-makejails/shiori \
    -o virtualnet=":<random> default" \
    -o nat \
    -o expose=8080
```

### Arguments

* `shiori_tag` (default: `14.3`): see [#tags](#tags).
* `shiori_ajspec` (default: `gh+AppJail-makejails/shiori`): Entry point where the `appjail-ajspec(5)` file is located.

### Volumes

| Name       | Owner | Group | Perm | Type | Mountpoint     |
| ---------- | ----- | ----- | ---- | ---- | -------------- |
| shiori-db  | 839   | 839   |  -   |  -   | /var/db/shiori |

## Tags

| Tag        | Arch     | Version            | Type   |
| ---------- | -------- | ------------------ | ------ |
| `14.3` | `amd64`  | `14.3-RELEASE` | `thin` |
| `15` | `amd64`  | `15` | `thin` |
