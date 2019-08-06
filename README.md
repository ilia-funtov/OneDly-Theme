# One-Day-Only (OneDly) Project Theme

This [Hugo](http://gohugo.io) theme is for documenting One-Day-Only (OneDly) projects. The theme renders a single page and is based on [Github project Page](https://themes.gohugo.io/github-project-landing-page/).


# Demo
A demo can be find here [...](https://github.com/cdeck3r/OneDly-Theme)

# Screenshot
![screenshot](...)

# Notable Differences

* Social media links as buttons at the top of the page
* Social media sharing links as buttons at the end of the page
* All posts on a single page as separated sections
* Post ordering by sec parameter, instead of date

# Customization

Check [config.toml](https://github.com/cdeck3r/OneDly-Theme/blob/master/exampleSite/config.toml) for available configuration. 

Below is a description for each of them.

The project name is specified as the title of the site.
```
title = "OneDly Project"
```

The project description follows in the `params` section.
```
[params]
    description = "Amazing project."
```

Other variables are
`author_name` the project author's name.
`author_url` link to the personal website of the project author.
`project_url` link to project url, e.g. the project's github repo 

**Note:** `description` and `author_name` are put into the site's meta data for author and the site description.

```
    author_name = "cdeck3r"
    author_url = "//cdeck3r.com"
    project_url = "//github.com/cdeck3r/OneDly-Theme"
```

Theme colors
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

