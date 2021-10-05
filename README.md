Notes to self...

## Non-intuitive part

Since GitHub ony allows serving GitHub Pages from root directory or a directory named `docs` (at least at this time, afaik), the actual content is served from another repository which is added as a submodule (`public` directory).

## Straightforward part

It uses Hugo (static site generator) to produce a "web servable" content in directory `public`.

## How to use
1. Use hugo to add new content
2. Run `hugo` to generate output
3. Go to root director and `git add`, `git commit -m "YOUR MESSAGE HERE"` and `git push`
4. When you want to publish the changes to `https://depy.github.io/`, go to public directory and do the same as in step 3 (add, commit, push)
5. Wait a minute for GitHub to reflect changes