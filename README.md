# [Geoelements Research Wiki Template](https://geoelements.org/wiki-template/)

The Geoelements Research Wiki uses  Markdown (.md) file format. The research wiki documents daily progress, literature review, methodology, and your thoughts on the results.

## Starting your wiki
Fork the [Research Wiki repo](https://github.com/geoelements/wiki-template) on GitHub to start your research wiki page. Prefix the repo-name as `wiki-`.

## Docsify

The wiki is rendered using  [Docsify](https://docsify.js.org/#/). 
Refer to [Docsify quick start](https://docsify.js.org/#/quickstart).

### Install

To install Docsify

```
npm i docsify-cli -g
```
### Compile and render wiki

From the root directory of the wiki run

```
docsify serve
```

This will typically serve a local version of the wiki on 
http://localhost:3000. Open the link on the browser to view the wiki.

## Customizing the wiki theme
The wiki title and links are defined in [index.html](index.html) file. 
Modify the following lines:
```
<meta name="description" content="Geoelements Research Wiki Template">
...
name: 'Geoelements Research Wiki Template',
...
repo: 'https://github.com/geoelements/wiki-template',
```

### Color scheme
You may also change the `themeColor`, but you also need to modify the 
`theme/vue.css` file to make the color schemes consistent. Current theme 
color is: `themeColor: '#bf5700'`. The following sections in the CSS needs to be updated:

```css
.sidebar-toggle {
  background-color: #fdf8e9;
}
.sidebar {
  background-color: #fdf8e9;
  color: #364149;
  background: #f9f7f0;
}
body {
  background-color: #f9f7f0;
}
```

## Folder/File organization

There are two main folders in the wiki `literature` and `research`. You may create other root folders like `code` or `theory` to discuss code or background theory. Feel free to create as many subfolders as you wish.

### File naming
In the `literature` section, always name the file as `yyyy-first-author.md` format. Always place images inside these folders following the same naming convention.

In the `research` section, create subfolders and use your judgment to 
organize the sections/subsections.

### Literature structure
Krishna recommends the following structure for your literature reviews.

```
## Title
> Authors
[Paper](link-to-paper)

> Keywords: #area #topic

### Terminology
New terms which you are unfamiliar

### Research questions 
Typically a bulleted list of questions

### Future research/unanswered questions
Questions unanswered by the paper

### Main findings
Explain their main research findings

### Methodology (optional)
Describe the critical procedure followed by the researchers.
```

You may also have subsections with a general description of state of the art in an area. These state-of-the-art or background materials don't have to follow the structure described above. The summary describes your understanding of the background and what's missing.

## Research workflow
Make changes to the wiki daily or at least once every couple of days. Summarize what you have done and write down the methods used and the results obtained, and most importantly, your thoughts on the results. The wiki is a living document that holds snapshots of your thought process. I recommend you use the active voice when writing the wiki. Think of the wiki as a mini-version or a subsection of your paper. Writing a manuscript would then be simply copying sections from the wiki and rearranging those sections.  When you have documented your results, create a PR on the GitHub repo and assign Krishna to review the doc. 

## Publishing
You are required to publish your research wiki to the GitHub Geoelements organization. However, you may choose to have your repo as either public or private. Note, once a paper is published, we require you to make the 
repo public as well.

## License
This research wiki is licensed under a [Creative Commons Attribution - NonCommercial 4.0 International License](https://creativecommons.org/licenses/by-nc/4.0/).