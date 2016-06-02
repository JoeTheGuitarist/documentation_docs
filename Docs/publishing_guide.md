# How to publish mbed documentation

This guide is intended for developers who are trying to add documentation to their projects. It details the tools we use (GitHub, docs.mbed.com and Markdown) and the scope of documentation.

For advice about writing your documentation, see [the writing guide](writing_guide.md).

## What to publish

Documentation about:

1. New things. 

1. Changes to existing things.

1. Deprecations. 

In other words: when you create a repository, or when you edit the code in an existing one, please create (or edit) documentation.

## Using GitHub and Markdown

Our documentation is written in Markdown and lives on GitHub:

1. MkDocs review [basic Markdown syntax](http://www.mkdocs.org/user-guide/writing-your-docs/) on their site.

1. Your docs should sit in the same GitHub repository as the code. So if you have a repo at github.com/ARMmbed/repo, you have two options:

    * Put an MD file in the root (https://github.com/ARMmbed/repo/readme.md).

    * Create a directory for your file (https://github.com/ARMmbed/repo/doc/readme.md). 

1. Feel free to create more than one MD file. But you should probably have readme.md as the main, because most people will look at it first. Then you can add files like API.md, changelog.md and deprecated.md.


## Publishing on docs.mbed.com

### Structuring your project

docs.mbed.com uses the [Mkdocs engine](http://www.mkdocs.org/). Read [their documentation](http://www.mkdocs.org/#getting-started) to learn about how they structure a project. 

<span class="notes">**Note:** We use the old YML format to organize pages. For example, this is the YML for the project you're currently reading:</span>
```
site_name: Documentation Guides

docs_dir: Docs

pages:
- ['index.md','Introduction to the Documentation Guides']
- ['publishing_guide.md', 'Publishing Guide', 'Publishing guide']
- ['style_guide.md', 'Writing Guides', 'Style guide']
- ['writing_guide.md', 'Writing Guides', 'Writing guide']
- ['product_names.md', 'Writing Guides', 'Product names']
```

In ``pages``, the elements are:

1. Page_name.md
1. Section title (not mandatory; the first page in this project isn't under a section title).
1. Page title.

<span class="tips">**Tip:** The table of contents on docs.mbed shows the page title from the YML *instead of* header 1; header 1 is shown only as part of the text. This prevents having two page titles - one from the YML and one from header 1 - appearing together in the table of contents.
<span class="images">![](Images/Header1.png)<span>The table of contents shows the page title from the YML, not header 1.</span></span>
</span>

### Publishing Markdown documentation

Documentation living on GitHub can be published on [docs.mbed.com](http://docs.mbed.com) using your mbed account:

1. Log into docs.mbed.com with your **developer.mbed.org** credentials.

    <span class="images">![](Images/DocsLogin.png)<span>Logging in</span></span>

1. You are taken to your dashboard.

1. Click **Import a Project**.

    <span class="images">![](Images/Import.png)<span>Import</span></span>

1. You have two importing options. Click **Manually Import Project**.

    <span class="images">![](Images/ManuallyImport.png)<span>Manually import</span></span>

1. Name your project and enter the GitHub repo URL.

    <span class="images">![](Images/ProjectDetails.png)<span>Project details</span></span>

1. Review the other options. The default values may well be all you need.

1. Click **Next**. You are taken to the project page.

1. The project tries to build a first version as soon as it's created. Click **Builds** to see the build's progress. 

    <span class="images">![](Images/ProjectHome.png)<span>Project home page</span></span>

1. When the build is done, you can click **View Docs** to see your project. 

<span class="tips">**Tip:** Your project's Admin page allows adding tags to your projects (as comma-seperated words). Tags help users find your documents, so we recommend using them.</span>

## Using docs.mbed features

docs.mbed offers a few features that aren't normally available on GitHub-flavoured Markdown.

### Including pages from other repos

If you're working with several repos, but want to publish all of their docs under one docs.mbed project, you can do that without duplicating pages.

1. Create your MD pages in whatever repos you want. Let's say ``source_repo/docs/source.md``.
1. In the repo you want to publish, create an empty MD or use an existing MD. For example ``publishing_repo/docs/publish.md``.
1. Get the link to the *raw* GitHub MD page from the source repo.
1. Paste the raw link in the publishing repo, preceded by an exclamation mark and held within curly brackets:

	``!{https://raw.githubusercontent.com/ARMmbed/source_repo/master/docs/source.md}``

1. Publish your repo.

Note that you cannot include parts of a page - you can only include the whole page.

You can see an example of this in the [uVisor_docs repo](https://github.com/ARMmbed/uvisor_docs).

<span class="notes">**Note:** you must republish your repo to show changes in the source repos.</span>


## Versioning your docs

docs.mbed supports publishing several versions of a project, and lets the users flip between versions as they read. 

### Creating branches for documentation

The basis for document versions is GitHub branches - so think before you name your branches, because that is what the users will see on docs.mbed.

These are my branches:

<span class="images">![](Images/Versions_on_GH.png)</span>

And this is what the version picker looks like when I build my versions:

<span class="images">![](Images/Versions_selection.png)</span>

### Selecting branches to publish

If you have more than one branch, docs.mbed will offer you a list of branches to build in **Dashboard > Admin > Versions**:

<span class="images">![](Images/Versions_on_docs_check.png)</span>

In the **Choose Active Versions** section, check the branches you want to build. You can remove them any time you like.

<span class="notes">**Note:** For an existing project, you may have to trigger a build to refresh the list of available versions.</span>

### Building a branch

In the project's **Build** page, the **Build version** drop-down lets you choose which version to build.

## Publishing Doxygen

docs.mbed will try to build Doxygen for your repository along with the regular documentation, so you should follow the previous section's instructions for publishing Markdown.

Note:

1. Please follow the general [Doxygen guidelines](http://www.stack.nl/~dimitri/doxygen/) to write your comments.
1. To generate a main page for your Doxygen, please create a markdown file in your repository's root called ``DOXYGEN_FRONTPAGE.md``.

## Markdown syntax on docs.mbed

The Markdown engine we use on docs.mbed - [MkDocs](http://www.mkdocs.org/user-guide/writing-your-docs/) - doesn't use exactly the same syntax as GitHub. This means that some things that look good on GitHub don't render correctly on docs.mbed. To get proper rendering on docs.mbed, you need to adjust your syntax a little.

Note that adjusting your syntax to match docs.mbed doesn't damage the text's appearance on GitHub, because GitHub supports both syntaxes.

### Code blocks within lists

If you want to have a code block in a numbered list, you can't use the fencing ``` syntax. Instead:

* You need an empty line before and after the code block.
* Use eight spaces (not Tab) to start the block.
* Use four more spaces (again - not Tab) for each indent the code requires.

Here's an example: 

<span class="images">![](Images/Code_Block.png)<span>Count the indents</span></span>

It renders as:

1. Create a `main.cpp` file with the following content:

        #include "mbed.h"

        DigitalOut led(LED1);

        int main()
        {
            while (true) {
                led = !led; // toggle led
                wait(0.2f);
            }
        }

1. Click  *Compile* and verify that your application builds as expected.  

### Lists with more than one level

If you want a list to render with more than one level of numbers or bullets, you need to use four spaces instead of Tab:

1. Level one first item
    1. Level two first item
    1. Level two second item
1. Level one second item

### Styling your docs

The docs.mbed engine supports the following syntax:

1. ``<span class="notes">This is what a note looks like</span>``
	<span class="notes">This is what a note looks like</span>
1. ``<span class="tips">This is what a tip looks like</span>``
	<span class="tips">This is what a tip looks like</span>
1. ``<span class="warnings">This is what a warning looks like</span>``
	<span class="warnings">This is what a warning looks like</span>
1. ``<span class="images">![](image_source)<span>caption</span></span>``
	<span class="images">![](Images/Flowers.jpg)<span>This is what an image looks like</span></span>

<span class="notes">**Note:** If you're reading this on GitHub you will see the default GitHub styling, not our styling.</span>

