# Bookmark utils

**My personal utility bookmarks, as a feed.**

## Subscribe

<p align="center">
	<a href="http://mhulse.github.io/bookmark-util/feed.xml">
		<img width="400" height="100" src="https://cloud.githubusercontent.com/assets/218624/6322833/282bc3c4-bad3-11e4-97b3-f7b7327d5249.png">
	</a>
</p>

## Bookmarklets

<a href="javascript:void(window.open('view-source:'+window.location.href));">Tab source</a>
<a href="javascript:location.href='http://fuckyeahmarkdown.com/go/?read=1&preview=0&showframe=0&u='+encodeURIComponent(document.location.href);">Readability→Markdown (raw)</a>

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
