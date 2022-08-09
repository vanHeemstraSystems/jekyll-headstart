# 400 - Update a Blog with Jekyll

Say we wish to make a post. How hard is it?

Let's checkout a branch and fire up Visual Studio Code:

```
$ git clone https://github.com/vanHeemstraSystems/vanheemstrasystems.github.io.git
$ cd vanheemstrasystems.github.io
$ ls 
README.md LICENCE index.html ...
$ code .
$ git branch
* main
$ git checkout -b feature/firstpost
Switched to a new branch 'feature/firstpost'
```

In Visual Studio Code, we can now create a new file called "**FirstPost.md**", add some content to it, and push it.

```
$ git add FirstPost.md
$ git commit -m "My first post"
[feature/firstpost b5ebdd6] My first post
1 file changed, 3 insertions(+)
create mode 100644 FirstPost.md
$ git push --set-upstream origin feature/firstpost
```

Nothing appears on [our blog](https://vanheemstrasystems.github.io) at first.  This is because pages is set to a branch spec (in our case "main"):

