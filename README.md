# Introduction
This is from official Odoo docker, just modified some for my developer experience.

# Tested Device
Im using Macbook Pro with M1 Pro, which ARM64 Arch

# Build your own image
Currently this is using build from Odoo Official, i will create later in project

# What can i use in this repo
1. DBeaver for opening/viewing the database
2. Debugpy for debuging in vscode

## Debugpy in vscode
this is for .vscode/launch.json
```
{
   "version":"0.2.0",
   "configurations":[
      {
         "name":"Python: Remote Attach",
         "type":"python",
         "request":"attach",
         "connect":{
            "host":"localhost",
            "port":5678
         },
         "pathMappings":[
            {
               "localRoot":"${workspaceFolder}",
               "remoteRoot":"."
            }
         ],
         "justMyCode":true
      }
   ]
}
```

# Running
1. Setup the env, just modify `.env.example` to `.env`
2. Setup the secret, just modify `secrets/pg_pass.example` to `secrets/pg_pass` (Actually you can use only .env, but i want to drop it as file when running the docker)
3. run docker compose with `docker-compose up -d`