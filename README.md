# Introduction
This is from official Odoo docker, just modified some

# Tested Device
Im using Macbook Pro with M1 Pro, which ARM64 Arch

# Build your own image
Currently this is using build from Odoo Official, i will create later in project

# What can i use in this repo
1. DBeaver for opening/viewing the database
2. Debugpy for debuging in vscode

# Debugpy in vscode
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

