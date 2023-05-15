---
authors: [Georg Makowski, Test Author, Anonymous]
title: Author pages
description: "Every page can have one or more authors"
subtitle: false
date: 2023-05-08T23:26:42+02:00 
menu:
  doc:
    identifier: authors
    name: Authors
    parent: siteelem
    pre: person
resources:
  - src: charles-etoroma-vkc1YLZ50yE-unsplash.jpg
    name: featured
    params:
      alt: Anonymous author
  - src: portrait.jpg
    name: portrait
    params:
      alt: Anonymous portrait    
categories: [author]
weight: 665
---

Every author listed in the front-matter field `authors` gets a personal page that lists her or his latest contributions.
{.p-first}
<!--more-->

Every author page is initially auto-generated by Hugo. To add personal Markdown content and images we need to create an explicit author page with a command in the project root like:

```sh {.left}
hugo new authors/your-name
```

This creates a new Markdown page with a set of front-matter parameters in {$content/authors/my-name/_index.md}:

```yaml {.left}
---
title: Your Name
description: Short description
subtitle: true
date: 2023-05-10T23:33:49+02:00
resources:
- src: 
  name: featured
  params:
    alt: Your Name
- src: 
  name: portrait
  params:
    alt: Your Name
draft: true
---
```

You can add your name as the `title` and a short description of your profession to the parameter `description`.

The author page needs a portrait of you as a quadratic image file for the source named `portrait`. This image is also used on all your pages and cards referencing them. It should have a side length of at least {${{< width/column 2 >}}}.

You can add a bigger image to your author page as the featured image.

**In the next beta release**: Social icons and parameters with links to social networks 