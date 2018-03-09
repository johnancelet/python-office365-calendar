# Office 365 Calendar API

## Install needed packages
```
pip install -r requirements.txt
``` 

## Create Microsoft Office App
You should set os variables: OFFICE_CLIENT_ID and OFFICE_CLIENT_SECRET. To get OFFICE_CLIENT_ID and OFFICE_CLIENT_SECRET you should follow the steps:
1. Login to https://apps.dev.microsoft.com/
2. Create an app, note your OFFICE_CLIENT_ID
3. Generate a new password (OFFICE_CLIENT_SECRET) under "Application Secrets" section
4. Under the "Platform" section, add a new Web platform and set "http://localhost:5000" as the redirect URL
5. Under "Microsoft Graph Permissions" section, add the below delegated permissions:  
    a) User.Read  
    b) Files.ReadWrite  
    c) Calendars.Read  
    d) Mail.Send  

## How to run
```
python ./src/main.py
```
