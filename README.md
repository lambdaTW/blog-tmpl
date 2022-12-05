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

# Test it
```shell
hugo server -D
```
