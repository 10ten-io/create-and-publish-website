Hello, I'm Alex and I will teach you how to quickly create your first website.

Before we start, make sure you have a [GitHub](github.com) account and [Visual Studio Code](https://code.visualstudio.com) installed.

At the end, you will have your own personal website.

First, let's understand what a website is in it's most basic form: an HTML file.

Open your file explorer and create a file called `index.html`. Open it with VSCode, write `Hello, I'm Alex` and save. Of course you should change by your name.

Now, open it with your browser. YAY! That's your first website.

Essentially, a website is an HTML file, that can be opened by browsers. Just like images can be opened by image editors, PDF files can be opened by PDF viewers, mp3 files can be opened by music players, and the list goes on. HTML files can be opened by browsers.

Now only you can see this file/website, because it is in your computer. To show this to your friends we will need to put it in a public machine, for example a GitHub server.

GitHub is a development platform that can store our files and serve them to the browser via `username.github.io` address. And much more that we will explore later.

To start, create a new repository to store the website files, and give it this name: `username.github.io`. Change `username` by your username in GitHub.

To send local files to GitHub we need Git, which is a terminal application shipped with OSX computers and most linux distributions. So you probably already have it, but if you don't, checkout the pre-work notes.

Git is used everyday by pretty much every developer in the world, so you better start using it. Good news is that we only need 5 commands today. You will write (or copy-paste) on a terminal running inside the same folder as `index.html`.

To toggle a terminal on the current folder in VSCode, hold the `control` or `ctrl` key and press the key `~` of your keyboard.

Only the first time when you create a new repository, you need to open a terminal on the `index.html` folder and run:

```
git init .
```

It initializes a local Git repository. Now, change `username` by your own GitHub username and run:

```
git remote add origin git@github.com:username/username.github.io.git
```
It links a GitHub remote repository to your local repository, so that you can exchange files between. It's a common convention to call it `origin` and we will use this name when we need to push changes.

Now, everytime you want to send changes to your website, you need to:
| command | description |
|---|---
| `git add index.html` | add files/changes to send to the remote repository |
| `git commit -m "nice description of what you did"` | group all changes with a nice description |
| `git push origin main` | push local commits to the remote `origin` on `main` branch |

If it asks for a username and password, type your GitHub username and password, and check the pre-work notes to learn how to stay authenticated with GitHub so that you don't have to type credentials every time you push changes.

Get used to those 3 commands, we will use them every day, just like every developer in the world!

If you followed those steps and didn't get any error, you should be able to see the index page on `username.github.io` after some seconds.

Take this moment to admire your accomplishment :)