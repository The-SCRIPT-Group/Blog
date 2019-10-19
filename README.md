# TSG Blog Repository

Those who have push access can add new content (basic rule).

&nbsp;

#### Initial configuration (First Time)

Go to [https://github.com/The-SCRIPT-Group/Blog](https://github.com/The-SCRIPT-Group/Blog) 

Choose the 'Fork' button on the right, to fork it to your account. Once that's done:

Click the **Clone or Download** green button on the right, copy the link to clipboard, go to your terminal and clone it to your PC by:

```bash
$ git clone https://github.com/your-profile/Blog.git
$ git remote add origin https://github.com/the-script-group/blog.git
```

*Note that 'your-profile' means your username on github, please don't blindly copy.*



#### More configuration (Needed every time)

#### Setting up environment

We need *ruby*, *gem* and *ruby-dev* packages (On Ubuntu atleast, please search for your system). Also ensure you have *git* installed

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

------

&nbsp;

#### Working on this blog

Do:

```bash
$ git clone https://github.com/The-SCRIPT-Group/Blog.git
```

Open the **Blog** folder on your system, in VSCode or any  other editor with folder and terminal support (makes your job easier, trust me. Always trust the person who makes the documentation).

&nbsp;

Once the folder is open, start the terminal in **Blog** and do:

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

***YYYY-MM-DD-NameOfPost.markdown*** and open in Typora (Markdown editor, please download)

At the top of the file, select Paragraph -> YAML Front Matter and put the following:

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

------

Original source: [Jekyll BLog](https://medium.com/20percentwork/creating-your-blog-for-free-using-jekyll-github-pages-dba37272730a)

