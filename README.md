# training-hugo-project

https://lotusdocs.dev/docs/overview/



Build a new site

Create a New Lotus Docs Site 


With Hugo installed, create a new Hugo project using the hugo new command:

```
hugo new site demo5 && cd demo5

```

Now initialize your project as a Hugo Module using the hugo mod init command:

```
hugo mod init demo5
```

```
git clone --depth 1 https://github.com/maniak-academy/workshop-theme themes/workshop-theme && rm -rf themes/workshop-theme/.git

git clone --depth 1 https://github.com/maniak-academy/workshop-content-demo content/docs && rm -rf content/docs/.git 
wget -O hugo.toml https://raw.githubusercontent.com/maniak-academy/workshop-toml/main/hugo.toml
```


Edit the hugo.toml configuration file to include the Lotus Docs theme and the Hugo Bootstrap module (lines 5 to 14 below):

baseURL = 'http://example.org/'
languageCode = 'en-us'
title = 'My New Hugo Site'

[module]
    # uncomment line below for temporary local development of module,
    # when using a 'theme' as a git submodule or git cloned files
    replacements = "github.com/maniak-academy/workshop-theme  -> workshop-theme "
    [[module.imports]]
        path = "github.com/maniak-academy/workshop-theme 
        disable = false
    [[module.imports]]
        path = "github.com/gohugoio/hugo-mod-bootstrap-scss/v5"
        disable = false




# training docs section 
        hugo new docs/.md

hugo new docs/Start/_index.md
hugo new docs/Start/Overview.md && sed -i 's/draft: true/draft: false/' Overview.md
hugo new docs/Prerequisite/_index.md
hugo new docs/Prerequisite/Prerequisite.md && sed -i 's/draft: true/draft: false/' Prerequisite.md
hugo new docs/Setup/_index.md
hugo new docs/Setup/Setup.md && sed -i 's/draft: true/draft: false/' Setup.md



hugo new docs/Overview.md && sed -i 's/draft: true/draft: false/' Overview.md
hugo new docs/Prerequisite.md && sed -i 's/draft: true/draft: false/' Prerequisite.md
hugo new docs/Setup.md && sed -i 's/draft: true/draft: false/' Setup.md
