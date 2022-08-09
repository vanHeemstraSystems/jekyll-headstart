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

Nothing appears on [our blog](https://vanheemstrasystems.github.io) at first.  This is because pages is set to a branch spec (in our case "main/master"):

![build-from-master](https://user-images.githubusercontent.com/1499433/183781093-25653bd6-578a-4b5c-84e2-5626faf532bb.png)

So let's Pull Request (PR) our changes back to main/master branch.  

We can go to the Pull Request (PR) page where we are prompted to make a PR:

![new-pull-request](https://user-images.githubusercontent.com/1499433/183781468-76c6da60-57a8-478e-ad52-35f99d801110.png)

Create the PR by clicking **Compare and pull request**.

![create-pull-request](https://user-images.githubusercontent.com/1499433/183781806-dff67380-c653-4a3c-9b7f-5ca4a337645e.png)





More ...
