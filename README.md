What is it?
-----------

Vim is a **great** text editor. The [Drew Neil](http://drewneil.com/) thinks so
and creates an awesome screencast series about Vim. That script allow to
download all [video archive](http://vimcasts.org/episodes/archive) in one shoot.

## Usage

```bash
./vimcasts.py --help
```

Download episodes 1-68
```bash
./vimcasts.py | tail -n +2 | head -n 68 > vimcast_url.txt
cat vim*.txt | parallel --gnu "wget {}"
```

## Notes
    This script only download m4v file on site. Not including other 10+ vimeo video embedded in the post.
    How to get them ?
        Open: http://vimcasts.org/feeds/quicktime.rss
        Search 'm4v' then copy links in the top nodes. Manually watch.

## Copyrights

Modified by Michael Zhuang
Created by Vital Kudzelka <vital.kudzelka@gmail.com>.

Licensed under the [MIT
License](http://mit-license.org/vitalk).
