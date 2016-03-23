# Lis.press repository

## How does it works?

I have a copy of this git repository on my virtual server on Digital Ocean. 

I use static generation to the `/public` directory and expose it with NGinx.

### Updates
Every time I need to update my site i pull my changes:
```
git pull
```

If i changed my config and there were **conflicts** in commit i stash changes, pull and then unstash:
```
git stash
git pull
git stash pop
```

And then I generate my static site:
```
hugo
```