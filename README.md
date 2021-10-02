# [Geoelements Research Wiki](https://geoelements.org/research-wiki-template/)

Geoelements Research Wiki template. The research wiki is written in  
Markdown (.md) file format. Fork the 
[Research Wiki repo](https://github.com/geoelements/research-wiki-template) on 
GitHub to start your own research wiki page. Talk to Krishna about the name of your repo.

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
repo: 'https://github.com/geoelements/research-wiki-template',
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

There are two main folders in the wiki `literature` and `research`. You may
create other root folders like `code` or `theory` to discuss aspects of 
code or background theory. Feel free to create as many subfolders as you 
wish.

### File naming
In `literature` section, always name the file as `yyyy-first-author-title.md` format. Follow the same naming convention for folders you create for the images. Always place images inside these folders. 

In the `research` section, create subfolders and use your judgement to 
organize the sections/subsections.

### Literature structure
We recommend the following structure for your literature reviews.

```
## Title
> Authors
[Paper](link-to-paper)

> Keywords: #area #topic

### Terminology
New terms which you are unfamiliar

### Research questions 
This is typically a bulleted list of questions

### Future research/unanswered questions
Questions unanswered by the paper

### Main findings
Explain their main research findings

### Methodology (optional)
Describe important procedure followed by the researchers.
```

## Publishing
You are required to publish your research wiki to the GitHub geoelements 
organization. However, you may choose to have your repo as either public 
or private. Note, once a paper is published, we require you to make the 
repo public as well.

## License
This research wiki is licensed under a [Creative Commons Attribution - NonCommercial 4.0 International License](https://creativecommons.org/licenses/by-nc/4.0/).