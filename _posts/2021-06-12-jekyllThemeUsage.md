---
title: jekyll usage
tag: manual
toc: true
---

#  side bar usage

_data/navigation.yml

```
docs:
  - title: Getting Started
    children:
      - title: "Quick-Start Guide"
        url: /docs/quick-start-guide/
      - title: "Structure"
        url: /docs/structure/
      - title: "Installation"
        url: /docs/installation/
      - title: "Upgrading"
        url: /docs/upgrading/
```

**Now you can pull these links into any page by adding the following YAML Front Matter.**

```
defaults:
  # _docs
  - scope:
      path: ""
      type: docs
    values:
      sidebar:
        nav: "docs"
```

**Note:** nav: "docs" references the docs key in _data/navigation.yml so make sure they match.

# post syntax

```
title: something
layout: archive, archive-taxonomy, search, single, splash, home, posts, categories, category, tags, tag
permalink:/fun/     #Theme entry
collection: fun
entries_layout: grid
classes: wide
toc: true 
toc_label: "My Table of Contents"
toc_icon: "cog"
listed: true
```

# location

Navigation : /_data/navigation.yml

Add navigation: /_config.yml

```
include:
  - .htaccess
  - _pages   #add this so it can recognize as posts or page
```

