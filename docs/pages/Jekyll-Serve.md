---
title: Jekyll Serve
layout: default
navigation_weight: 8
---
# Jekyll Serve

**Jekyll** server statements may be entered from the *Integrated Terminal* view of your target repo's open `docs` folder in **Visual Studio Code**. 

{% include toc-flammarion.md %}

## Visual Studio Code

From the main menu of **Visual Studio Code**, engage the `File`, `New Window` feature ...

And, navigate to the local (location) of your **first targeted** repo that you wish to operate upon.

- Select the `docs` folder of your **first targeted** repo.

**Note One**. Because the Jekyll server we will be serving (.md) files from the `pages` subfolder of your repo's `docs` folder by default ...

Be sure to target the `docs` folder of your **first targeted** repo selection for opening.

**Note Two**.  You may always set up a separate instance of the Jekyll server from the `root` folder of your **first targeted** repo selection ...

If you need to perform an operation over any of the other files or folders of your **first targeted** repo's local `root` folder.

## Jekyll Version

To check the version of Jekyll you have installed *globally* on your development machine ...

-- Type the following *shortcut* `-v` statement derived from the Jekyll `--version` switch, as follows:

```liquid
{% raw %}
jekyll --v
{% endraw %}
```
Returns,

```liquid
{% raw %}
jekyll 3.4.3
{% endraw %}
```

**Note Three**. **Git Hub** publishes a current list of dependency versions for the *Git Hub Pages* dependency, the *Ruby* dependency, the *Jekyll* dependency, and others.

Before including any dependency in the `Bundle install` or `Bundle update` task for your repo ...

Please check the current dependency list over at **Git Hub** prior to applying any dependencies to your repo.

## Default Port = 4000

To engage the Jekyll server via a separate tab through your Chrome browser window ...

- Type the following Jekyll statement into the *Integrated Terminal* view of the open `docs` folder of your **first targeted** repo in Visual Studio Code, as follows:

```liquid
{% raw %}
jekyll serve --watch --baseurl ""
{% endraw %}
```

The above Jekyll statement will *automatically* open up a new `tab` in your Chrome browser window via the `serve` command and the accompanying set of designated *switches*.

## Jekyll Switches

In this case, the `--watch` and `baseurl` switches are engaged.

The `watch` switch shows no *immediate parameter* ...

While, the `baseurl` switch shows the the empty string `""` as its one *immediate parameter*.

**Note**. The following URL is the default address of the Jekyll server instance, as follows:

```liquid
{% raw %}
http://localhost:4000/
{% endraw %}
```

## Open Sez-A-Me

Served locally, you will now see the `docs` folder of your **first targeted** repo open in a separate instance of the Jekyll server via the default address of the automatically opened Chrome browser window tab.

This will allow the end-user (developer) to make changes to the underlying (.md) pages ...

And, then view those changes locally via their development machine **PRIOR** to uploading the changes to the *Git Hub server farm* via **Git Hub Desktop**.

**Note**. If you wish to host multiple `doc` repos over multiple instances of the Jekyll server through separate tabs of your Chrome browser window ...

Then, you must manually dedicate the port in your opening Jekyll `serve` command statement.

## Set Port = 4001

The `--port` switch in Jekyll requires the target port as its immediate parameter, as follows:

```liquid
{% raw %}
--port 4001
{% endraw %}
```

In the **first targeted** repo example above, the Jekyll command statement defaulted to a `switch` of `--port 4000` *implicitly*.

To include a 2nd tab and 2nd instance of the Jekyll server within our now open Chrome browser window ... 

- We will need to select a **second targeted** repo to open, and

- We will have to *explicitly* call the `--port 4001` switch in our instantiating Jekyll command statement.

**Note**. For further review, see the Jekyll `--help` switch.

## Jekyll Help

To engage the Jekyll `--help` switch from an open Terminal window ...

- Type the following Jekyll statement into the *Integrated Terminal* view of your open `docs` folder in Visual Studio Code, as follows:

```liquid
{% raw %}
jekyll --help
{% endraw %}
```

## Jekyll Docs

To start a local server for the Jekyll documentation ...

- Simply type the following Jekyll statement into the *Integrated Terminal* view of your open `docs` folder, as follows:

```liquid
{% raw %}
jekyll docs
{% endraw %}
```

And, up pops a local iteration of **Jekyll Docs** served through the implicit default `--port 4000`.

## Serve Switches

To review the optional switches for the `serve` command in Jekyll ...

- Type the following Jekyll statement into the *Integrated Terminal* view of your open `docs` folder in Visual Studio Code, as follows:

```liquid
{% raw %}
jekyll help serve
{% endraw %}
```

## Serve Statement #2

To engage the Jekyll server via a separate tab through your Chrome browser window ...

- Type the following Jekyll statement into the *Integrated Terminal* view of the open `docs` folder of your **second targeted** repo in Visual Studio Code, as follows:

```liquid
{% raw %}
jekyll serve --watch --baseurl "" --port 4001
{% endraw %}
```

Now, manually open up a new `tab` in your Chrome browser window and set the address to the following URL ...

```liquid
{% raw %}
http://localhost:4001/
{% endraw %}
```

You will now see the **second targeted** repo open in a separate instance of the Jekyll server under a separate tab of your Chrome window browser.

**Note**. If you wish the new and separate tab of your Chrome browser window to open automatically ...

Then, set the following `-o` *shortcut* derived from the Jekyll `--open` switch, as well.

As follows,

```liquid
{% raw %}
jekyll serve --watch --baseurl "" --port 4001 -o
{% endraw %}
```

## New Subtitle

More to come ...

```liquid
{% raw %}
Enjoy the successful output!
{% endraw %}
```

## Last Subtitle

Place the introducing line of text ie.) the 'tagline' here ...

```liquid
{% raw %}
Enjoy the successful output!
{% endraw %}
```

{% include sources-and-uses.md %}

### External Sources

- The [Project Source Links](https://mminail.github.io/Jekyll/Source-Jekyll-Links.htm){:title="Click to Visit the Source Links page of the Jekyll Lessons Project at GitHub pages"}{:target="_blank"} page of the Jekyll Lessons Project. Published by © 2017 [Mminail.github.io](https://mminail.github.io/){:title="Click to Visit the Concept Library of the Medical Marijuana Initiative of North America - International Limited, an Arizona Benefit Corporation"}{:target="_blank"}.




