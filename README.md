# TSG Blog Repository

Those who have push access can add new content directly (I assume you know git push).

&nbsp;

#### Initial configuration (First Time)

Go to [https://github.com/The-SCRIPT-Group/Blog](https://github.com/The-SCRIPT-Group/Blog) 

Choose the 'Fork' button on the right, to fork it to your account. 

&nbsp;

Once that's done:

Go to your account ke repos, you'll find 'Blog'. Go to that.

Click the **Clone or Download** green button on the right, copy the link to clipboard, go to your terminal and clone it to your PC by:

```bash
$ git clone CTRL+SHIFT+V
$ git remote add tsg https://github.com/the-script-group/blog.git
```

*Note that 'your-profile' means your username on github, please don't blindly copy.*



#### Setting up environment

We need *ruby*, *gem* and *ruby-dev* packages (On Ubuntu atleast, please search for your system). Also ensure you have *git* installed. Also download Typora from [https://www.typora.io/](https://www.typora.io/)

To check ruby version, do:

```bash
$ ruby -v
```

&nbsp;

To check gem version, do:

```bash
$ gem -v
```

&nbsp;

To install Jekyll (first time, if you don't have), do:

```bash
$ gem install jekyll bundler
```

Once done installing, check by:

```bash
$ jekyll -v
```

&nbsp;

These steps are for first-time setup only.

------

&nbsp;

#### More steps (Needed every time)

If you did the above the first time successfully (DRC dude), continue with these:

In your terminal, do these *to fetch latest changes from main repo (mandatory)*:

```bash
git fetch tsg gh-pages
git reset --hard tsg/gh-pages
git clean -fdx
```

ALWAYS DO THIS BEFORE EDITING, ELSE YOUR CHANGES WILL GET OVERWRITTEN!

&nbsp;

------

&nbsp;

#### Working on this blog

Open the **Blog** folder on your system which you cloned, in VSCode or any  other editor with folder and terminal support (makes your job easier, trust me. Always trust the person who makes the documentation).

&nbsp;

Once the folder is open, start your terminal inside **Blog** folder and do:

```bash
Blog$ bundle exec jekyll serve 
```

Site should be up and running on http://127.0.0.1:4000/. It'll show up in the terminal prompt as well.

------

So, we have our blog running on our system. Cool. 

&nbsp;

1. **_posts:** This is the folder that has all our blog posts. Each of these posts should be a *markdown file* (with a .markdown extension) and should be included within this folder for it to be listed in your blog.
2. **_site:** This files in this folder are responsible for compiling your blog. You basically have different blog posts, images, pages lying in different folders. The files in _sites folder bring them together and publish it as a website. **(Not needed for blogging)**
3. **_config.yml:** This file contains your site’s variables such as title, your usernames, urls etc. **(Not needed for blogging)**
4. **about.md:** This is just a markdown file that contains data to be published in your about section. **(Not needed for blogging)**
5. **gemfile**: gemfile contains all the dependencies for this site. Meaning you are using jekyll. And within jekyll, you are using it’s default theme called ‘Minima’. The gem file specifies such info.
6. **index.md:** contains info that is visible in the home page of your blog.

&nbsp;

Go to _posts, and make a new file in the format:

***YYYY-MM-DD-NameOfPost.markdown*** and open in Typora.

At the top of the file, select Paragraph -> YAML Front Matter and put the following compulsorily:

layout: post

title: "Name this blog post"

date: YYYY-MM-DD HH:MM:SS +0530

categories: ctgry1 subctgry1

&nbsp;

Add your text and stuff after this matter. After making changes, run:

```bash
$ jekyll serve
```

after stopping the previous running instance with CTRL+C

&nbsp;

------

Push changes like you'd do in git:

```bash
$ git add .
```

```bash
$ git commit -m "Describe the post in short"
```

```bash
$ git push origin gh-pages
```

This'll make changes to your forked repo, not the main TSG one. To do that, do the following:

1. Go to [https://github.com/the-script-group/blog](https://github.com/the-script-group/blog), click 'New Pull Request'

2. Click the 'compare across forks' button on the right

3. On the right section, there's 'head repository' dropdown. Choose **your Blog repo** from the list. Keep the rest same.

4. Click Create Pull Request, on the next page, add some comment, and click Create Pull Request

5. Wait for your changes to get merged. Else just spam Akhil or Ritom or Aniket 

   &nbsp;

------

Original source: [Jekyll BLog](https://medium.com/20percentwork/creating-your-blog-for-free-using-jekyll-github-pages-dba37272730a)

