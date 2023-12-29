# training-hugo-project

The following code builds a simple doc tutorial service that lets you build a training course for anything. It's based off of https://lotusdocs.dev with the addition of VSCode and a Terminal

### Note Only works on ARM silicon right now ##

## Prerequists 
* Docker / Docker desktop Installed
* Git /Github access
* Fork the following repo https://github.com/maniak-academy/training-hugo-project.git

## Build in Docker
If you have forked the repo then you can clone it into your own machine. 


```
git clone https://github.com/maniak-academy/training-hugo-project.git
```

Jump into the directory and take a look at the docker-compose.yaml file, this will run docker and deploy hugo server and run it with the content in your repo.

It will deploy 
1. Hugo Server port 1313
2. TTYD Termainl Server 7681
3. VSCode Server (coming soon)
4. Quacaomole Server (coming soon)

Exectue the following command to spin the docker up

```
docker-compose up -d 
```

To shut it down run 

```
docker-compose down
```

Now you can go to http://localhost:1313 or http://localhost:7681 and you are set


## How to add content

Add content using markup language in the content/docs folder.

