---
currentMenu: home
---

# Template by Frontender
![](https://getfrontender.com/assets/images/brand/frontender-light-bg.png)
<br/><br/><br/><br/>

## Installation process
1. Run ```curl -OS http://couscous.io/couscous.phar``` to install couscous.
2. Run ```php couscous.phar preview``` to render the docs.
3. Navigate to http://127.0.0.1:8000/ or http://localhost:8000/ to view the docs.

## Usage

To use the template, set it up in your `couscous.yml` configuration file:

```yaml
template:
    url: https://github.com/getfrontender/Template-ReadTheDocs
```

## Configuration

Here are all the variables you can set in your `couscous.yml`:

```yaml
# Base URL of the published website
baseUrl: http://username.github.io/project

# Used to link to the GitHub project
github:
    user: myself
    repo: my-project

title: My project
subTitle: This is a great project.

# The left menu bar
menu:
    items:
        home:
            text: FAQ
            # You can use relative urls
            relativeUrl: doc/faq.html
        foo:
            text: Another link
            # Or absolute urls
            absoluteUrl: https://example.com
```

Note that the menu items can also contain HTML:

```yaml
home:
    text: "<i class=\"fa fa-github\"></i> FAQ"
    relativeUrl: doc/faq.html
```

## Menu

To set the current menu item (i.e. highlighted menu item), set the `currentMenu`
key in the Markdown files:

```markdown
---
currentMenu: home
---

# Welcome
```
