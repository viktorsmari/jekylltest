
---
title: frontpage
---

### testing

## 1
<ul class="posts">
{% for post in site.posts limit: 20 %}
  <div class="post_info">
    <li>
         <a href="{{ site.baseurl }}{{ post.url }}">{{ post.title }}</a>
         <span>({{ post.date | date:"%Y-%m-%d" }})</span>
    </li>
    <li>site.baseurl: {{ site.baseurl }} , post.url: {{ post.url }}
    </li>
    </div>
  {% endfor %}
</ul>

## 2

{% for post in site.posts %}	
    [{{ post.title }}]({{ post.url }}) {{ post.date | date: "%B %e, %Y" }} {{ post.category }} {{ post.url }}
{% endfor %}	

## 3
site.baseurl {{ site.baseurl }}
site.url {{ site.url }}

## Welcome to GitHub Pages

You can use the [editor on GitHub](https://github.com/viktorsmari/jekylltest/edit/master/index.md) to maintain and preview the content for your website in Markdown files.

Whenever you commit to this repository, GitHub Pages will run [Jekyll](https://jekyllrb.com/) to rebuild the pages in your site, from the content in your Markdown files.

### Markdown

Markdown is a lightweight and easy-to-use syntax for styling your writing. It includes conventions for

```markdown
Syntax highlighted code block

# Header 1
## Header 2
### Header 3

- Bulleted
- List

1. Numbered
2. List

**Bold** and _Italic_ and `Code` text

[Link](url) and ![Image](src)
```

For more details see [GitHub Flavored Markdown](https://guides.github.com/features/mastering-markdown/).

### Jekyll Themes

Your Pages site will use the layout and styles from the Jekyll theme you have selected in your [repository settings](https://github.com/viktorsmari/jekylltest/settings). The name of this theme is saved in the Jekyll `_config.yml` configuration file.

### Support or Contact

Having trouble with Pages? Check out our [documentation](https://help.github.com/categories/github-pages-basics/) or [contact support](https://github.com/contact) and we’ll help you sort it out.
