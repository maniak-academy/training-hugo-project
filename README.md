# training-hugo-project

https://lotusdocs.dev/docs/overview/



Build a new site

Create a New Lotus Docs Site 


With Hugo installed, create a new Hugo project using the hugo new command:
```
hugo new site demo4 && cd demo4

```

Now initialize your project as a Hugo Module using the hugo mod init command:

hugo mod init demo4


git clone https://github.com/maniak-academy/workshop-theme themes/workshop-theme 


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


        hugo new docs/example-page.md


docker run --rm \
  --name vscode-server \
  --hostname vscode \
  -p 8000:8000 \
  -e VSCODE_SERVE_MODE=serve-local \
  ahmadnassri/vscode-server:latest