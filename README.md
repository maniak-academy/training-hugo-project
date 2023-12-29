# training-hugo-project

The following code builds a simple doc tutorial service that lets you build a training course for anything. It's based off of https://lotusdocs.dev with the addition of VSCode and a Terminal

## Prerequists 
* Docker / Docker desktop Installed
* Git /Github access

## Build in Docker
The first we are need to do is fork the repo into your own repository.

```

```

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

## run 

```
hugo server -D
```

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


docker run -p 4200:4200 -e SIAB_PASSWORD=W3lcome098! -e SIAB_SUDO=true sspreitzer/shellinabox:latest


https://github.com/sspreitzer/shellinabox-container-image