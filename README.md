Jujutsu Link
============

I've grown quite used to having (`git link
<something>`)[https://github.com/msiebuhr/git-link] around when needing to
point to something in git repository, and was missing that in `jj`.

```sh
# Link to the repository
jj-link
https://github.com/msiebuhr/jujutsu-link

# Link to a particular commit
jj-link -r xk
https://github.com/msiebuhr/jujutsu-link/commit/ab43e20c55ae8f9202290e1356a0d60b58d1d4f4

# Link to a particular file
jj-link LICENSE 
https://github.com/msiebuhr/jujutsu-link/-/blob/d779e3a1734ac8d2c74cb37f086ed3d4223800bf/LICENSE
```

Installation
------------

There's no dependencies; drop it in your path somewhere. I use `~/.local/bin`.

Ideas
-----

 - Support `--repository` for consistency
 - Allow linking to particular lines in files. Perhaps re-use vim syntax: `jj-link <filename> +123`?
 - Add `--open` for automatically opening in a browser.
 - Propose for inclusion in Jujutsu's ['forge' roadmap]((https://martinvonz.github.io/jj/latest/roadmap/#forge-integrations)
 - Adapt to whatever <https://github.com/martinvonz/jj/issues/3001> ends up with
