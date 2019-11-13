---
title: File Setup
layout: default
excerpt: Place the introducing line of text ie.) the 'tagline' here ...
description: Issue, Rule, Analysis, Conclusion = IRAC
repo: Jekyl Lessons Project
ver_date: 11-12-19
navigation_weight: 8
categories: template
---
# File Setup

When fully configured, a Jekyll site will consist of a total of (8) files and folders in the root directory of the repo and another (10) files and subdirectories in the docs folder of the repo.

![MMI™ Flammarion Logo Badge](../assets/ico/ms-icon-70x70.png)

## Table O Contents

- TOC
{:toc}

## The Repo Root Directory

The root directory of the repo houses the docs folder from which all **Git Hub Pages** magic is rendered, specifically through the pages subdirectory of the docs folder.

## Setting the Remote Jekyll Server

The remote Jekyll server can be set after creating a new repository up at Git Hub.

Locally, the master synch from local to remote requires simply an index dot md file and a default layout file, plus the docs folder.

Both the default layout file which is placed in the `_layouts` subdirectory within the docs folder and the index dot md file which is placed directly in the docs folder may be synched up to the Git Hub - Jekyll server master via the **Git Hub For Mac** program.

Once synched, a trip to the settings of your new repo will allow you to select a theme ( Cayman ) after declaring the docs folder will be the house where the magic required to render **Git Hub Pages** will be performed.

After successfully committing the changes to the local master and then synching with the remote master, the remote master will place a config dot yaml file within your new docs folder.

The config dot yaml file is the configuration file for your repo and will be addressed before we `Bundle install`.

For right now, we will accept the declaration of the Cayman theme as given by the remote master within the now well placed config dot yaml file.

**Note**. Don't forget to synch with the remote master again in order to see the "Add Jekyll - Cayman Theme" show up in the history timeline of the master branch of your local repo.

## Working From The Local Master

Eventually, we will establish a local working branch from the master, but for now we will continued to synch our local master with the remote master up at Git Hub for each change until we are finished wth the **File Setup**.

### Gemfile and Gemfile dot lock

The Gemfile is established from a template, and can be formed with simple copy and paste, as follows:

```liquid
{% raw %}
source "https://rubygems.org"
ruby "2.4.1"
#
# Date of this Update to Gem-template file ver 07-29-2017
#
# The Gemfile is where you manage Jekyll versioning.
#
# For example ...
#
# sass "3.4.25"
# 
# Hello! This is where you manage which Jekyll version is used to run.
#
# Use the following instruction list to instantiate an instance of the Jekyll Server on your development machine ...
#
# First ... you will need to install the 'Ruby Version Manager' onto your development machine.
#
# And, then install a copy of 'Ruby ver 2.4.1' with the help of your new 'Ruby Version Manager'
#
# You will then need to install a copy of the 'Gem Bundler' program using a Terminal command, as follows:
#
# gem install bundler
#
# Once you have successfully installed the 'Gem Bundler' program to your development machine ...
#
# You may run the following command from a Terminal prompt to check the current version installed, as follows:
# 
# bundler --version
#
# And, you may run the following command from a Terminal prompt to check the location of your new Bundler version, as follows:
#
# which bundler
#
# If you need to upgrade your version of the 'Gem Bundler' program, run the following command from a Terminal prompt:
#
# gem update bundler
#
# Once you have successfully installed the 'Gem Bundler' program to your development machine ...
#
# You may now install the local Jekyll Server with the following Terminal command ...
#
# gem install jekyll
#
# Be sure to always preface your work at the Terminal with the following Ruby command:
#
# rvm use 2.4.1
#
# In order to ensure you are working on the correct gem.
#
# Use the following command at the Terminal to double-check ...
#
# which jekyll
#
# Note. You only need to install the Bundler and Jekyll gems one time on your development machine.
#
# It is not necessary to install the Bundler and Jekyll gems every time you create a separate repo. 
#
# A Gemfile ( with no extension ) will be automatically created in the root directory of your new repo.
# 
# If not, create a Gemfile ( with no extension ) and import the contents of this template.
#
# Finally, run the following command from the Terminal prompt of the root directory of your new repo to load the directives of this template.
#
# bundle install
#
# When you want to use a different version of Jekyll, make the changes below.
#
# And, then save the file and run the following command from the Terminal prompt of the root directory of your repo.
#
# bundle update github-pages
#
# Bundler will then install the Jekyll version you have described.
#
# Next, optionally run the command 'jekyll' from the Terminal command line with the command ...
#
# bundle exec jekyll serve
#
# This will help ensure the proper Jekyll version is up and running!
#
# To start the Jekyll server, type the following command at the Visual Studio Code integrated terminal window from the /docs directory of your repo:
#
# jekyll serve --watch --baseurl ""
#
# Then, navigate to: http://localhost:4000/ with your browser
#
# Note. The Gemfile and Gemfile dot lock files should be created upon the installation of the Bundler gem.
# 
# The purpose of the Gemfile and Gemfile dot lock files is to inform Bundler about the gem requirements of your GitHub pages website.
# 
# If your website does not have the the Gemfile and Gemfile dot lock files sitting in the root directory of the repo ( NOT in the /docs website subdirectory! ) ...
#
# Then, you can omit the 'bundle exec' command from above and just run the 'jekyll serve' command.
#
# Happy Jekyll-ing!
#
# Note. If you want to use GitHub Pages, comment out the following gem 'jekyll'
#
# gem 'jekyll', '3.4.3'
#
# If you want the option to run Jekyll docs locally ... enable the following line here, and type 'jekyll docs' from the Terminal window of any repo
gem 'jekyll-docs', '3.4.3'
#
# Note. The default theme for new Jekyll sites is 'minima'.
# gem "minima", "~> 2.0"
#
# You may change this to anything you like.
gem "jekyll-theme-cayman"
#
# Note. To upgrade, run `bundle update github-pages` from the command line.
gem 'github-pages', group: :jekyll_plugins
#
# If you have any Jekyll plugins, put them here ...
group :jekyll_plugins do
   gem "jekyll-feed", "~> 0.6"
end
#
gem 'github-markdown'
gem 'jekyll-gist'
gem 'jekyll-coffeescript'
gem 'jekyll-paginate'
#
gem 'jekyll-seo-tag'
#
gem 'jekyll-sitemap'
#
# Note. Windows does not include zoneinfo files, so bundle the tzinfo-data gem
gem 'tzinfo-data', platforms: [:mingw, :mswin, :x64_mingw, :jruby]
#
{% endraw %}
```

**Note**. The **Gemfile** has no suffix. The **Gemfile dot lock** file will be established when the Terminal command `Bundle install` is performed at the end of **File Setup**.

### dot Git and dot Git Ignore

The **dot Git** file is established at the time of repo creation up at Git Hub.

Upon cloning via download to the **Git Hub For Mac** program, a license file, a Read Me file, and a **dot Git Ignore file** can be established, as well.

The **dot Git Ignore** file may be established from a local template, and can be formed with simple copy and paste, as follows:

```liquid
{% raw %}
# Ignore Visual Studio temporary files, build results, and files generated by popular Visual Studio add-ons
#
# Template Dtd 07-30-17
#
# Jekyll Files
_site
.sass-cache
.jekyll-metadata
#
# User-specific files
*.suo
*.user
*.userosscache
*.sln.docstates
#
# User-specific files (MonoDevelop/Xamarin Studio)
*.userprefs
#
# Build results
[Dd]ebug/
[Dd]ebugPublic/
[Rr]elease/
[Rr]eleases/
x64/
x86/
bld/
[Bb]in/
[Oo]bj/
[Ll]og/
#
# Visual Studio 2015 cache/options directory
.vs/
# Uncomment if you have tasks that create the project's static files in wwwroot
#wwwroot/
#
# MSTest test Results
[Tt]est[Rr]esult*/
[Bb]uild[Ll]og.*
#
# NUNIT
*.VisualState.xml
TestResult.xml
#
# Build Results of an ATL Project
[Dd]ebugPS/
[Rr]eleasePS/
dlldata.c
#
# DNX
project.lock.json
artifacts/
#
*_i.c
*_p.c
*_i.h
*.ilk
*.meta
*.obj
*.pch
*.pdb
*.pgc
*.pgd
*.rsp
*.sbr
*.tlb
*.tli
*.tlh
*.tmp
*.tmp_proj
*.log
*.vspscc
*.vssscc
.builds
*.pidb
*.svclog
*.scc
#
# Chutzpah Test files
_Chutzpah*
#
# Visual C++ cache files
ipch/
*.aps
*.ncb
*.opendb
*.opensdf
*.sdf
*.cachefile
*.VC.db
*.VC.VC.opendb
#
# Visual Studio profiler
*.psess
*.vsp
*.vspx
*.sap
#
# TFS 2012 Local Workspace
$tf/
#
# Guidance Automation Toolkit
*.gpState
#
# ReSharper is a .NET coding add-in
_ReSharper*/
*.[Rr]e[Ss]harper
*.DotSettings.user
#
# JustCode is a .NET coding add-in
.JustCode
#
# TeamCity is a build add-in
_TeamCity*
#
# DotCover is a Code Coverage Tool
*.dotCover
#
# NCrunch
_NCrunch_*
.*crunch*.local.xml
nCrunchTemp_*
#
# MightyMoose
*.mm.*
AutoTest.Net/
#
# Web workbench (sass)
.sass-cache/
#
# Installshield output folder
[Ee]xpress/
#
# DocProject is a documentation generator add-in
DocProject/buildhelp/
DocProject/Help/*.HxT
DocProject/Help/*.HxC
DocProject/Help/*.hhc
DocProject/Help/*.hhk
DocProject/Help/*.hhp
DocProject/Help/Html2
DocProject/Help/html
#
# Click-Once directory
publish/
#
# Publish Web Output
*.[Pp]ublish.xml
*.azurePubxml
# TODO: Comment the next line if you want to checkin your web deploy settings
# but database connection strings (with potential passwords) will be unencrypted
*.pubxml
*.publishproj
#
# Microsoft Azure Web App publish settings. Comment the next line if you want to
# checkin your Azure Web App publish settings, but sensitive information contained
# in these scripts will be unencrypted
PublishScripts/
#
# NuGet Packages
*.nupkg
# The packages folder can be ignored because of Package Restore
**/packages/*
# except build/, which is used as an MSBuild target.
!**/packages/build/
# Uncomment if necessary however generally it will be regenerated when needed
#!**/packages/repositories.config
# NuGet v3's project.json files produces more ignoreable files
*.nuget.props
*.nuget.targets
#
# Microsoft Azure Build Output
csx/
*.build.csdef
#
# Microsoft Azure Emulator
ecf/
rcf/
#
# Windows Store app package directories and files
AppPackages/
BundleArtifacts/
Package.StoreAssociation.xml
_pkginfo.txt
#
# Visual Studio cache files
# files ending in .cache can be ignored
*.[Cc]ache
# but keep track of directories ending in .cache
!*.[Cc]ache/
#
# Others
ClientBin/
~$*
*~
*.dbmdl
*.dbproj.schemaview
*.pfx
*.publishsettings
node_modules/
orleans.codegen.cs
#
# Since there are multiple workflows, uncomment next line to ignore bower_components
# (https://github.com/github/gitignore/pull/1529#issuecomment-104372622)
#bower_components/
#
# RIA/Silverlight projects
Generated_Code/
#
# Backup & report files from converting an old project file
# to a newer Visual Studio version. Backup files are not needed,
# because we have git ;-)
_UpgradeReport_Files/
Backup*/
UpgradeLog*.XML
UpgradeLog*.htm
#
# SQL Server files
*.mdf
*.ldf
#
# Business Intelligence projects
*.rdl.data
*.bim.layout
*.bim_*.settings
#
# Microsoft Fakes
FakesAssemblies/
#
# GhostDoc plugin setting file
*.GhostDoc.xml
#
# Node.js Tools for Visual Studio
.ntvs_analysis.dat
#
# Visual Studio 6 build log
*.plg
#
# Visual Studio 6 workspace options file
*.opt
#
# Visual Studio LightSwitch build output
**/*.HTMLClient/GeneratedArtifacts
**/*.DesktopClient/GeneratedArtifacts
**/*.DesktopClient/ModelManifest.xml
**/*.Server/GeneratedArtifacts
**/*.Server/ModelManifest.xml
_Pvt_Extensions
#
# Paket dependency manager
.paket/paket.exe
paket-files/
#
# FAKE - F# Make
.fake/
#
# JetBrains Rider
.idea/
*.sln.iml
#
# compiled output
/dist
/tmp
/out-tsc
#
# Node dependencies
/platforms
/node_modules
#
# IDEs and editors
/.idea
.project
.classpath
.c9/
*.launch
.settings/
*.sublime-workspace
#
# IDE - VSCode
.vscode/*
!.vscode/settings.json
!.vscode/tasks.json
!.vscode/launch.json
!.vscode/extensions.json
#
# misc
/.sass-cache
/connect.lock
/coverage
/libpeerconnection.log
npm-debug.log
testem.log
/typings
#
# e2e
/e2e/*.js
/e2e/*.map
# Gradle
*.iml
.gradle
/local.properties
/.idea/workspace.xml
/.idea/libraries
/build
/captures
.externalNativeBuild
#
{% endraw %}
```

**Note**. The above **dot Git Ignore** file is a derivative of the **Visual Studio** template shown at the time of repo creation up at Git Hub.

So far, we have discussed and shown (4) of the eight files and folders required in the root directory of the repo for a successful Jekyll experience, they are ...

1. dot Git
1. dot Git Ignore
1. Gemfile
1. Gemfile dot lock

The other (4) files and folders are, as follows:

1. Docs folder
1. favicon.ico
1. License file
1. Readme dot md

Now, we must establish our **Git Hub Pages** remotely after committing at a minimum, the docs folder, the index dot md file, and the a default layout file and folder.

### Default Layout

The default layout file and `_layouts` folder may be established from a local template, and can be formed with simple copy and paste.

**Note**. The `_layouts` subdirectory is placed under the `docs` folder.

Here is the code required to establish an effective default layout file.

```liquid
{% raw %}
<!DOCTYPE html>
<html lang="en-us">
  <head>
    <meta charset="UTF-8">
    <title>{{ page.title | default: site.title }}</title>
    <meta name="description" content="{{ page.description | default: site.description | default: site.github.project_tagline }}"/>
    <meta name="viewport" content="width=device-width, initial-scale=1">
    <meta name="theme-color" content="#157878">
    <link href='https://fonts.googleapis.com/css?family=Open+Sans:400,700' rel='stylesheet' type='text/css'>
    <link rel="icon" type="image/x-icon" href="favicon.ico">
    <link rel="stylesheet" href="{{ '/assets/css/style.css?v=' | append: site.github.build_revision | relative_url }}">
    {% seo %}
  </head>

  <body>
    <section class="page-header">

      <h1 class="project-name">{{ site.title | default: site.github.repository_name }}</h1>

      <h2 class="project-tagline">{{ site.description | default: site.github.project_tagline }}</h2>

      {% if site.github.is_project_page %}
        <a href="{{ site.github.repository_url }}" class="btn">View on GitHub</a>
      {% endif %}

      {% include nav.htm %}

      {% if site.show_downloads %}
        <a href="{{ site.github.zip_url }}" class="btn">Download .zip</a>
        <a href="{{ site.github.tar_url }}" class="btn">Download .tar.gz</a>
      {% endif %}

    </section>

    <section class="main-content">
      <!-- \{\% include page-banner.htm \%\} 
        <hr class='green-groove' /> -->

      {{ content }}

      {% include icon-github-footer.htm %}

      <!-- <hr class='green-groove' />
       \{\% include footer.htm \%\} -->
    </section>

    {% if site.google_analytics %}
      <script type="text/javascript">
        (function(i,s,o,g,r,a,m){i['GoogleAnalyticsObject']=r;i[r]=i[r]||function(){
        (i[r].q=i[r].q||[]).push(arguments)},i[r].l=1*new Date();a=s.createElement(o),
        m=s.getElementsByTagName(o)[0];a.async=1;a.src=g;m.parentNode.insertBefore(a,m)
        })(window,document,'script','//www.google-analytics.com/analytics.js','ga');

        ga('create', '{{ site.google_analytics }}', 'auto');
        ga('send', 'pageview');
      </script>
    {% endif %}

  </body>
</html>
{% endraw %}
```

#### Discussion

Notice there are a number of "includes" in the above layout template in addition to the double curly brace ( moustache ) call for primary content.

The corpus of your markdown file will be rendered where the content moustache statement is placed within the template.

Whereas, the individual content of each include will be placed in the same respective location where the include is placed on the layout template.

## The Includes

More to come ...

## Markdown External Hyperlink

- Live Link

[Medcoin™ Crypto Currency Project: Ping-back Home Page](https://rwebaz.github.io/Medcoin-Crypto-Currency-Project/){:target="_blank"}

- The Code

```liquid
{% raw %}
[Medcoin™ Crypto Currency Project: Ping-back Home Page](https://rwebaz.github.io/Medcoin-Crypto-Currency-Project/){:target="_blank"}
{% endraw %}
```

## Raw Code

```liquid
{% raw %}
`...`
{% endraw %}
```

***

**Source**: [Instructional Jekyll Tips n Vids by Cloud Cannon](https://learn.cloudcannon.com/){:target="_blank"}. Published by © 2017 [Cloudcannon.com](https://www.cloudcannon.com){:target="_blank"}.
