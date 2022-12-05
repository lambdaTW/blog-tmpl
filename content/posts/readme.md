+++
title = "Read me"
date = "2022-12-05T18:56:25+08:00"
author = ""
authorTwitter = ""
cover = "https://d33wubrfki0l68.cloudfront.net/c38c7334cc3f23585738e40334284fddcaf03d5e/2e17c/images/hugo-logo-wide.svg"
tags = ["intro", "profile"]
keywords = ["", ""]
description = ""
showFullContent = false
readingTime = false
hideComments = false
color = ""
+++

# How to create this project
```shell-script
hugo new site blog-tmpl
cd blog-tmpl
git init
echo ".hugo_build.lock" >> .gitignore
echo "resources/" >> .gitignore
git submodule add -f https://github.com/panr/hugo-theme-terminal.git themes/terminal
```

## Edit config.toml
```toml
baseURL = '/'
languageCode = 'en-us'
title = 'My Blog'
theme = 'terminal'

[params]
  centerTheme = true

[languages]
  [languages.en]
    [languages.en.params.logo]
      logoText = "Blog"
      logoHomeLink = "/"
```

# How to create new post
```shell
hugo new posts/<name-of-post>.md
$EDIT content/posts/<name-of-post>.md
```
