# Content management on GitHub

The skill share formerly known as "Jekyll"

---

# What is content management on the web?

* Creating, editing and publishing content
* Systems for presenting content (style, look and feel)

---

# Content Management Systems (CMSs)

## Run your own

* WordPress [link](https://wordpress.org)
* Drupal [link](https://www.drupal.org)
* many others ...

These systems cover blogging and more general content publishing.

## Use a platform

* Wordpress.com [link](https://en.wordpress.com)
* Tumblr [link](https://www.tumblr.com)
* many others ...

These platforms are focused on blog publishing.

---

# What's wrong?

## Run your own

* Security
* Maintenance
* Cost (Time and Money)


## Use a platform

* Limited publishing features
* Limited presentation features
* Limited control over data

---

# Enter Jekyll

[http://jekyllrb.com/]([http://jekyllrb.com/)

* A "static site generator"
* It's all text - no database, for example
* Originally designed around blogging, like WordPress
* Made by hackers, for hackers

---

# Why use a static site generator?

* No security considerations
* No ongoing maintenance costs
* Low to zero cost in time and money

---

# When to use a static site generator

* Content that is read only
* Content that is not regularly updated/changed
* Content that is not user generated, or user specific

## Examples

* [Open Data Handbook](http://opendatahandbook.org)
* [Open Data Index](http://index.okfn.org)
* [Open Knowledge Labs](http://okfnlabs.org)

---

# But ... Jekyll

* Made by hackers, for hackers
* Text editors, command line, good times!
  * ... if you write code

**How can we get the benefits of using static sites, and still have a reasonable workflow for content management?**

---

# GitHub <3 Jekyll

[https://github.com/](https://github.com/)

* GitHub has built-in support for "building" Jekyll sites
* GitHub provides an interface for collaboration
* GitHub hosts static sites for free

---

# Benefits for content management

* Open by default
* We are already on GitHub for many projects
* No security considerations
* No servers to setup
* No ongoing maintenance costs
* Low to zero cost in time and money

---

# Demystification

We now know why we'd use a "static site generator" like Jekyll.

We also have an idea that GitHub can serve as a platform for hosting such sites, and managing their content.

However, GitHub is a collaboration platform for code. We need to demystify it so we can understand it for publishing content.

---

# A GitHub glossary

* **Repository**: Basically, the contents of a project, or just: "a project"
* **Commit**: The rest of us call that "Save"
* **Pull Request** (also **PR**): A request to the person who runs a repository to merge your changes to into the "canonical version"
* **Fork** (*verb*): Create your own copy of a repository
* **Fork** (*noun*): A copy of a repository
* **Branch**: A special area of a repository where content can be found

---

# Code is text

**The code that people store and share on GitHub is just text**.

* [Example](https://github.com/okfn/opendatacensus/blob/feature/database/app.js): This file is a set of commands for a machine, but it is also just a file with text in it.

Colloborating on code via GitHub is not all that different to collaborating on content via other platforms. It is just a bit more *formal*.

Without directly using the specialized terminology, on GitHub we:

* Create projects to keep our content
* Allow others to make copies of our content
* Accept changes to our content from others via a **formal request procedure**
* Save changes to our own content and thereby update our projects

---

# All about Markdown

Markdown is a set of additional characters used with normal "plain text".

To start, you just need to know:

* The "#" character is used for headings
* The "*" character is used for emphasis
* The "-" character is used to list things
* Write content like you'd normally write an email, and mix these characters

[Here is the guide to Markdown syntax](http://daringfireball.net/projects/markdown/syntax)

**An example**:

    # Hi!

    Oh, I *almost* forgot, today I **have** to:

    - Eat broccoli
    - Go swimming
    - Drink coffee

---

# Where are we now?

We've covered:

* Why we'd use a "static site generator"
* Why we'd use GitHub as a content publishing platform
* What GitHub terminology actually means
* The basics of Markdown

---

# Let's do something

[https://github.com/](https://github.com/)

* Login to GitHub if you haven't already

---

# Create a web page on GitHub

We are going to create a web page hosted on GitHub.

* Create a new repository
* Go to "Settings"
* Go to "Launch automatic page generator"
* Add a Tagline
* Remove the default markdown from the text area
* Write some markdown!
* Go to "Continue to layouts"
* Choose a layout by clicking an item in the slider across the top
* Click "publish page"
* Visit the page

That was just for fun :).

---

# Show your participation in this skill share

* Go to https://github.com/pwalsh/github-content and **fork** this repository
* Add a new file to "_participants"
* Create *front matter* for this file
* Add a sentence under the front matter using Markdown
* Commit
* Make a Pull Request

---

# What did we just do?

* Made a personal copy of a project
* Added a new file of content to that project, in our own personal copy
* Asked the project owner to accept our own changes into the "official" project copy

---

# Resources

* Sam Smith's [excellent guide for contributing to the Open Data Handbook](http://opendatahandbook.org/contribute/)

---

# Participants

<ul>
  {% for person in site.participants %}
  <li>
      <strong>{{ person.name }}:</strong><br />
      {{ person.content }}
  </li>
  {% endfor %}
</ul>
