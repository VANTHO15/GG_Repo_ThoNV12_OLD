# ThoNV begin
Bước 1: copy folder bin bỏ vào C:\Users\thonv12
Bước 2:  vào env sửa path và them đường dẫn vào
![image](https://github.com/VANTHO15/GG_Repo_ThoNV12/assets/56969447/342bf754-fe44-4461-b769-ca7367a4dbf8)
Bước 3: Tạo 1 folder bất kì, vào cmd
Bước 4: gõ đường dẫn bên dưới vào để tải source và liên kết repo, -b là branch gì, -m là trỏ tới manifest xml
+ repo init -u https://github.com/VANTHO15/GG_Central_Repo_XML.git -b main -m ThoNV.xml --no-clone-bundle
+ Khi này cần đăng nhập thì user và pass
Bước 5:  Mình cần tải folder nào về thì tải thôi, lệnh như dưới
repo sync --no-clone-bundle -d docs
repo sync --no-clone-bundle -d port test_port
# ThoNV begin


# repo

Repo is a tool built on top of Git.  Repo helps manage many Git repositories,
does the uploads to revision control systems, and automates parts of the
development workflow.  Repo is not meant to replace Git, only to make it
easier to work with Git.  The repo command is an executable Python script
that you can put anywhere in your path.

* Homepage: <https://gerrit.googlesource.com/git-repo/>
* Mailing list: [repo-discuss on Google Groups][repo-discuss]
* Bug reports: <https://bugs.chromium.org/p/gerrit/issues/list?q=component:repo>
* Source: <https://gerrit.googlesource.com/git-repo/>
* Overview: <https://source.android.com/source/developing.html>
* Docs: <https://source.android.com/source/using-repo.html>
* [repo Manifest Format](./docs/manifest-format.md)
* [repo Hooks](./docs/repo-hooks.md)
* [Submitting patches](./SUBMITTING_PATCHES.md)
* Running Repo in [Microsoft Windows](./docs/windows.md)
* GitHub mirror: <https://github.com/GerritCodeReview/git-repo>
* Postsubmit tests: <https://github.com/GerritCodeReview/git-repo/actions>

## Contact

Please use the [repo-discuss] mailing list or [issue tracker] for questions.

You can [file a new bug report][new-bug] under the "repo" component.

Please do not e-mail individual developers for support.
They do not have the bandwidth for it, and often times questions have already
been asked on [repo-discuss] or bugs posted to the [issue tracker].
So please search those sites first.

## Install

Many distros include repo, so you might be able to install from there.
```sh
# Debian/Ubuntu.
$ sudo apt-get install repo

# Gentoo.
$ sudo emerge dev-vcs/repo
```

You can install it manually as well as it's a single script.
```sh
$ mkdir -p ~/.bin
$ PATH="${HOME}/.bin:${PATH}"
$ curl https://storage.googleapis.com/git-repo-downloads/repo > ~/.bin/repo
$ chmod a+rx ~/.bin/repo
```


[new-bug]: https://bugs.chromium.org/p/gerrit/issues/entry?template=Repo+tool+issue
[issue tracker]: https://bugs.chromium.org/p/gerrit/issues/list?q=component:repo
[repo-discuss]: https://groups.google.com/forum/#!forum/repo-discuss
