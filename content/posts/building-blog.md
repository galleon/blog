+++ 
draft = false
date = 2021-05-01T18:11:14+02:00
title = "Updating my blog"
tags = ['hugo', 'blog']
categories = ['coding']
+++
I have an extremely small cache memory and it is always a pain to retrieve how to update my blog. So I thought that a blog post on how to update my blog could be useful.
Let's start.

First create a new post:
```bash
cd blog;  hugo new posts/my-new-post.md
```
With your preferred text editor, add some interesting content. You can keep only a basic header as below.
```yaml
+++
draft = true
date = 2021-05-01T18:11:14+02:00
title = "My new blog post"
tags = ['hugo', 'blog']
categories = ['coding']
+++
```
Then, test it using:
```bash
 hugo server -D
```
and open `http://localhost:1313/`. Once you feel it is ready to publish
{{< highlight bash >}}
hugo -D
./deploy.sh
{{< /highlight >}}
And do not forget to push your changes:
```bash
git add config.toml content/posts/my-new-post.md
git commit -m "My new post"
git push
```
