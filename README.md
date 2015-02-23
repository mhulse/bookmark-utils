# Bookmark utils

**My personal utility bookmarks, as a feed.**

## Local development

Install missing gems:

```bash
$ cd repo/
$ bundle install
```

Or, update gems:

```
$ bundle update
```

Execute jekyll and serve:

```bash
$ bundle exec jekyll serve
```

View your locally-hosted site at <http://localhost:4000>.

## Clean Firefox bookmark HTML export regex

Find:

```regex
<DT><A href="(.*)">(.*)</a>
```

Replace:

```regex
- title: "$2"\n  desc:\n  uri: "$1"
```
