### How to use **Tokenizer** task

Follow the below steps to upload this task to your account:

1. Download the [zip file](https://github.com/UCrypton/VSOTasks/archive/master.zip).
2. Extract the zip file
3. Open command prompt and navigate to the folder: **Tokenizer\x.x.x** where x.x.x is the version number for the task like 1.0.0
4. Install ```tfx-cli``` utility
```
> npm install -g tfx-cli
```
5. To avoid providing credentials in every command, you can login once. Currently supported credential types are Personal Access Tokens and basic auth. [Create a personal access token](http://roadtoalm.com/2015/07/22/using-personal-access-tokens-to-access-visual-studio-online) and paste it in the login command
```
> tfx login
Copyright Microsoft Corporation
Enter collection url > https://youraccount.visualstudio.com/DefaultCollection
Enter personal access token >
logged in successfully
```
You can alternatively use basic auth by passing ```--authType basic``` (read [Configuring Basic Auth](https://github.com/Microsoft/tfs-cli/blob/master/docs/configureBasicAuth.md)).
6. Upload the task to your account:
```
> tfx build tasks upload ./
```
7. Once the task is uploaded, you would be able to view this task under **Utility** section of tasks 
