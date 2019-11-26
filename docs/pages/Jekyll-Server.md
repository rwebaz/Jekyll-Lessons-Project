---
title: Jekyll Server
layout: default
excerpt: Place the introducing line of text ie.) the 'tagline' here ...
hint: Place the intro paragraph ie.) the 'hypothesis' here ...
repo: Jekyll-Lessons-Project
ver_date: 11-26-19
navigation_weight: 8
categories: page
---
{% include toc.md %}

## How to engage the Jekyll Server locally

> **Hint**. {{ page.hint }}

More to come ...

### How To Start The Local Jekyll Server In Mac Os Sierra

From the **Integrated Terminal** in **Visual Studio Code**...

```liquid
{% raw %}
jekyll serve --watch --baseurl ""
{% endraw %}
```

Returns ...

Files are served locally at this URL ...

```liquid
{% raw %}
http://127.0.0.1:4000/
{% endraw %}
```

## Optional Configuration

```liquid
{% raw %}
jekyll serve --watch --baseurl "/docs"
{% endraw %}
```

Returns ...

Files are served at this URL ...

```liquid
{% raw %}
http://127.0.0.1:4000/docs/
{% endraw %}
```

## Ruby from Source

Some people have two copies of Ruby on their development machine.

One instance being the original 'system' configuration that came bundled with their machine.

And, the other instance relative to their administrative instant User account.

Click To Download Ruby from Source.

[Ruby](https://www.ruby-lang.org/en/downloads/){:target="_blank"}

## Ruby Macports

Click To Review the Ruby Macports 2nd Instance Page.

Learn how to make a **Binary Archive** from source.

[Ruby Macports 2nd Instance](https://mminail.github.io/Homebrew/Ruby-Macports-2nd-Instance.htm){:target="_blank"}

## More Stuff

```html
<li>Go to your locally configured repo in the Finder</li>

<li>Right click over the folder name</li>

<li>Expose the Services menu</li> 

<li>Open a 'new Terminal at folder'</li>

<span>Once a Terminal window is open with the directory pointing to the folder of your repo ...</span>

<ol type="1" start="5">

**Tip**. Once you have entered the local Jekyll server start command at the Terminal prompt and hit enter ...

You may then subsequently simply scroll up the Terminal history to accept the command in the future.

<ol type="1" start="6">

<li>Now, open up your chrome browser</li>

<li>And, type this address in the URL location bar of your browser window ... <kbd>http://localhost:4000/</kbd></li>

<br />

<li>Hit the <kbd>Enter</kbd> key to navigate to the local rendering of your repo</li>

## Other Stuff

Jekyll is best served as a Ruby gem.

[Click To Download Jekyll as a Ruby gem](https://rubygems.org/gems/jekyll){:target="_blank"}
```

## Raw Code Finish

```liquid
{% raw %}
<span lang='es' title='Sp. for 'Finish''>Finito! <i class='icon-large icon-flower'></i></span>
{% endraw %}
```

## Last Subtitle

More to come ...

***

**Note**. The above synopsis was derived from an article written by Cloud Cannon [[1](#CLOUDCANNON){:.red}].

1. {:#CLOUDCANNON}[Instructional Jekyll Tips n Vids by Cloud Cannon](https://learn.cloudcannon.com/){:title="Click to Review Instructional Jekyll Tips n Vids by Cloud Cannon"}{:target="_blank"}

***

{% include patreon-link.md %}
