# quickstart 

The [hugo docs getting started section](https://gohugo.io/getting-started/) has a  
[quickstart](https://gohugo.io/getting-started/quick-start/) guide. This project  
follows the guide, committing each step up to the add-content section.


```
baseURL = 'https://example.org/'
languageCode = 'en-us'
title = 'Arion (you said it wrong)'
theme = 'ananke'
```

https://github.com/theNewDynamic/gohugo-theme-ananke#readme
add the ananke theme by copying config in themes/ananke/exampleSite/config.toml to root config.toml



## Hosting 
https://gohugo.io/hosting-and-deployment/hosting-on-github/
changed the hugo version from 0.141.0 to 0.135.0

## Notes 
[Hugo in 100 Seconds](https://www.youtube.com/watch?v=0RKpf3rK57I)  
Files from the video are in `.100s/`  

Used as a CMS allowing author's to create content in markdown, then rendered to html based 
on the structure of the file system. File System Routing.

Developers use templates to control how the content is presented. Go Templates to 
interopolate and transform data from content.

example templates in .100s/laytouts/

templates can: 

define variables:
```
{{ $hello := value}}
```
form loops:
```
{{ range .Pages }}

{{ end }}
```
fetch:
```
{{ $myData := getJSON "url" }}
```

all kinds of other functionality (os.Stat, now, md5, Math)

Templates are organized into hierarchy of layouts
minimize code duplication, while maximizing flexibility

Content types with Taxonomy system
Easy to implement menus, tags, categories without plugins
used on Cloudflare documentation, smashing magazine and fireship.io

Get Started:
Install
`hugo new site my-blog`
Create a new web page by writing markdown in the content folder
OR use cli to generate it `hugo new end-the-fed.md` which provides a
default schema that can be customized in the arhcetypes folder.

Can install a theme or structure it from scrath using layouts (folder).

Syntax Highligting
Image Processing
Internationalization
Shortcodes