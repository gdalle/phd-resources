---
permalink: /tutorials/zotero/
title: Zotero
sidebar:
    nav: "tutorials"
---

As a researcher, once you reach a certain number of articles and books, simply storing them as PDF files in nested folders is no longer enough. [Zotero](https://www.zotero.org/) is a bibliography manager that lets you easily organize and exploit your academic sources.

It is a really intuitive and well-built piece of software, which allows you to

- Automatically download references and all their info (title, authors, date, journal, etc.) without entering all of that manually
- Store your sources along with the associated full texts, but also add notes or extract annotations directly from the PDFs
- Easily search through all of your articles, organize them into collections or mark them with tags
- Insert citations into Word or LaTeX documents and generate bibliographies in whatever style you need to use

... and lots of other cool things I will show you later!

If all you need to do is generate a bibliography without storing articles for future use, you can also try the web tool [ZoteroBib](https://zbib.org/).

## Setting up Zotero

To get started quickly, take a look at [this guide](https://www.zotero.org/support/quick_start_guide) explaining the main features of the software. A more extensive documentation is available [here](https://www.zotero.org/support/).

If you are stuck with something, take a look at the [FAQ](https://www.zotero.org/support/frequently_asked_questions), the (more extensive) [knowledge base](https://www.zotero.org/support/kb) or ask your question on the [forum](https://forums.zotero.org/discussions).

### Installation

Zotero has two main building blocks:

- The standalone app, which is responsible for storing and handling your references
- The browser connector, which allows you to directly download papers and metadata into the app when you visit a journal's webpage

Both of these things can be installed from the [downloads page](https://www.zotero.org/download/). However, I recommend installing the [development build](https://www.zotero.org/support/dev_builds) instead of the stable version, since this one comes with an awesome feature: an integrated PDF viewer and editor that plays well with the rest of the app.

Installation support is available [here](https://www.zotero.org/support/installation).

### Synchronization

If you use Zotero from multiple computers, or even if you just want an online backup of your collections, you may want to use the built-in [synchronization features](https://www.zotero.org/support/sync). There are two aspects to synchronization: data and files.

As soon as you create a [Zotero account](https://www.zotero.org/user/register/) and connect it to the standalone app, all of your items, notes, tags and collections will be synced to the Zotero server free of charge, and with no space limitation. However, this does not extend to PDF attachments. And since these can take up a lot of space, you have several options to choose from:

- Put the [Zotero base directory](https://www.zotero.org/support/preferences/advanced) on your computer inside your Google Drive or Dropbox folder. I do not recommend this option since you may have problems with concurrent file writing (when Zotero and your cloud provider both try to access the files at the same time).
- Connect Zotero to a WebDAV-compatible cloud service from [this list](https://www.zotero.org/support/kb/webdav_services). Unlike the first option, in this case the synchronization is handled by Zotero itself, which prevents concurrent access.
- If you don't have a (compatible) cloud service, buy a [Zotero file storage](https://www.zotero.org/storage?id=storage), and possibly have your university pay you back.

### Plugins

Zotero comes with a variery of community-developed [plugins](https://www.zotero.org/support/plugins) which can make your workflow much easier. Usually, they are available as GitHub repositories: to install a plugin,

1. On the GitHub repository, go to the `Releases` page, select the latest one and download the `.xpi` file.
2. In the Zotero app, go to `Tools > Add-Ons` and click on the wheel to select `Install Add-On From File`, then select the `.xpi` you just retrieved.
3. Restart Zotero.

#### Text editing

- [Word Processor Plugins](https://www.zotero.org/support/word_processor_integration) are necessary to use Zotero from Word, LibreOffice or Google Docs
- [Better BibTex](https://retorque.re/zotero-better-bibtex/) is essential if you want to use Zotero for Markdown or LaTeX editing.
- [Zotero MdNotes](https://argentinaos.com/zotero-mdnotes/) is nice if you want to edit Markdown notes outside of Zotero. See my [Foam tutorial](foam.md) for more details to set it up.

#### Managing attachments

- [Zotfile](http://zotfile.com/) is useful for renaming attachments, but most importantly it allows you to extract annotations and highlighted text from PDF files and store them as Zotero notes.
- [Zotero Folder Import](https://github.com/retorquere/zotero-folder-import) can help you transition from a folder-based file management system to Zotero.
- [Zotero Storage Scanner](https://github.com/retorquere/zotero-storage-scanner) scans your library for missing or broken attachments.

#### Automatic metadata

- [Zotero DOI Manager](https://github.com/bwiernik/zotero-shortdoi) downloads missing DOIs. A DOI is a unique identifier given to every scientific article at publication.
- [Zotero CitationCounts](https://github.com/eschnett/zotero-citationcounts) computes citation counts from various databases, for instance to help you prioritize readings.

#### Other

- [Zutilo](https://github.com/wshanks/Zutilo) provides additional editing features that are missing from the main app.

## Daily use

### Import

There are several ways to [add items](https://www.zotero.org/support/adding_items_to_zotero) to your library:

- When you're on a publisher's webpage, click the `Zotero Connector` button in your browser to save the paper and its metadata.
- In the Zotero app, click `Add item by identifier` (the magic wand) and enter an ISBN, DOI, PMID or Arxiv ID to automatically import a paper.
- Copy the BibTex info and go to `File > Import from clipboard`.
- Enter the metadata manually.

When using the first two methods, Zotero will try to find a full-text associated with the article, either from the publisher's website (if you have access to it) or from some other place on the internet. However, this doesn't always work, in which case you have to find the PDF yourself and [add it manually](https://www.zotero.org/support/attaching_files) to the item, for instance via drag and drop.

Be careful not to add items to your library using only the PDF, since Zotero will often fail to extract correct metadata from the full text file, especially for preprints or journals with little formatting.

### Notes, tags and connected papers

The Zotero interface allows you to store lots of additional objects alongside each paper:

- [Notes](https://www.zotero.org/support/notes), which you may use to remember the key points of an article, or to extract highlights and annotation with Zotfile.
- [Tags](https://www.zotero.org/support/collections_and_tags#tags), which can help you label sources depending on your needs. I often use tags such as #to-read or #not-interesting, but they can also serve to identify the bibliography bibliography for one of your projects.
- [Related items](https://www.zotero.org/support/related), which allow you to link library items with each other to remember connections (such as citation networks or common ideas).

### Collections and saved searches

Once your library becomes large enough, you will want to subdivide it into categories, or [collections](https://www.zotero.org/support/collections_and_tags#collections). They are like folders on your computer, except that one Zotero item can be in several collections without needing to be duplicated. Personally, my collections reflect a division into fields and sub-fields, but others use them to separate their different projects.

If you want a collection that automatically includes relevant items, you should go with a [saved search](https://www.zotero.org/support/searching) instead. This allows you to keep a collection updated with all the sources satisfying given criteria (for instance those that have a given word in their abstract).

### Export

A list of references is only useful if you put it somewhere. Luckily, Zotero offers plenty of options for [export](https://www.zotero.org/support/creating_bibliographies): you can either output your bibliography as a text, choosing from a wide array of predefined citation formats, or you can create a BibTex `.bib` file for use within LateX documents. 

### Group libraries

To collaborate with colleagues on a list of sources, the easiest way is to create a [group](https://www.zotero.org/support/groups). This makes it possible to share collections, items, notes and so on with other Zotero users

### Various tricks

A full list of [tips and tricks](https://www.zotero.org/support/tips_and_tricks) is available in the docs, but here are my favorites:

- When an item is selected, you can see the collection it appears in by pressing `Alt`.
- A right click on the title of a reference allows you to choose the case.
- To use LaTeX symbols in the fields of a paper (like the title), just add the #LaTeX tag to the Zotero item.

## Other sources

Here are two tutorials in French made by PhD friends, from which I heavily drew to make this one:

- 🇫🇷 [Cap sur Zotero](http://la.moyenagiste.fr/cap-sur-zotero) by La Moyenâgiste
- 🇫🇷 [Gérez votre bibliographie avec Zotero](https://zestedesavoir.com/tutoriels/2041/gerez-votre-bibliographie-avec-zotero/) by Qwerty

Be sure to check out the French-speaking 🇫🇷 [Zotero blog](https://zotero.hypotheses.org/) as well.
