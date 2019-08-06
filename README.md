# One-Day-Only (OneDly) Project Theme

This [Hugo](http://gohugo.io) theme is for documenting One-Day-Only (OneDly) projects. The theme renders a single page and is based on [Github project Page](https://themes.gohugo.io/github-project-landing-page/).

# Demo
A demo can be found here [...](https://github.com/cdeck3r/OneDly-Theme)

# Screenshot
![screenshot](https://github.com/cdeck3r/OneDly-Theme/blob/master/images/screenshot.png)

# Notable Differences

* Social media links as buttons at the top of the page
* Social media sharing links as buttons at the end of the page
* All posts on a single page as separated sections
* Post ordering by sec parameter, instead of date


# Quick Start

1. install [Hugo](http://gohugo.io) 
1. Create a new site: `hugo new site myproject`
1. Change dir: `cd myproject`
1. Add the OneDly theme: `git submodule add https://github.com/cdeck3r/OneDly-Theme.git themes/onedly`
1. Start server: `hugo server -D -t onedly` 

# Customization

Check [config.toml](https://github.com/cdeck3r/OneDly-Theme/blob/master/exampleSite/config.toml) for available configuration. Below is a description for each of them.

### Project Specification Parameters

The project name is specified as the title of the site.
```
title = "OneDly Project"
```

The project description follows in the `params` section.
```
[params]
    description = "One-Day-Only (OneDly) project documentation."
```

Other variables within the `[params]` section are 

* `author_name` the project author's name.
* `author_url` link to the personal website of the project author.
* `project_url` link to project url, e.g. the project's github repo 

**Note:** `description` and `author_name` are used as the site's meta data for author and description within the html header.

Examples

```
    author_name = "cdeck3r"
    author_url = "//cdeck3r.com"
    project_url = "//github.com/cdeck3r/OneDly-Theme"
```

### Section Ordering

The project documentation may consists of several files indicating different sections. All files need to be placed in `myproject\content\post` directory. 

One may create a new section using `hugo new post/about.md`. It is recommended to start with an About section. In the file's front matter specify 

```
+++
title = "About"
date = "2019-02-28"
sec = 1
+++
```

The `sec` variable defines the position on the site. `sec = 1` lets the About section appear at the beginning right below the description and social media links. In the next section, created by the command above, you may specify a larger number, e.g. `sec = 4`. This positions this new section after the About section and before a section with `sec = 5` or larger. If you do not specify a `sec` variable ordering falls back to default ordering by the date sourced from the front matter. Information on ordering are found in [Hugo's documentation](https://gohugo.io/templates/lists/#default-weight-date-linktitle-filepath).


### Social media

A user may specify links to well-known social media sites shown at the top of the page. In `config.toml` the section `[social]` lists the supported social media links. If the variable in this section specifies the user's account name, the corresponding button linking to the social media site will appear on the page.

The exampleSite's [config.toml](https://github.com/cdeck3r/OneDly-Theme/blob/master/exampleSite/config.toml) for examples.

### Theme colors

Standard theme colors are 

```    
    first_color="#f8f8f8"
    first_border_color="#e7e7e7"
    first_text_color="#333"

    second_color="white"
    second_text_color="#333"

    header_color="#f8f8f8"
    header_text_color="rgb(51, 51, 51)"

    header_link_color="#777"
    header_link_hover_color="rgb(51, 51, 51)"

```

