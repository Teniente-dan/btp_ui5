# btp_ui5

## Verify html5 app repo is bound to a certain service
### HTML5 Applications
    0. Download an app repo {app}

### Cloud Foundry -> Space -> instances
    00. any instance in the list -> ... -> view Dashboard

### destination -> {app}-destination-service
**destination-content**

    1. Service Keys
        comfujicargarcomprobantes-destination-content-comfujicargarcomprobantes-destination-service-credentials
        "xsappname": "clone0479b8098ef8413bbaeab6758442d28b!b76300|destination-xsappname!b62"
            
> 0479b8098ef8413bbaeab6758442d28b = **0479b809-8ef8-413b-baea-b6758442d28b**.approuter.registrocomplementos-0.0.1 (**downloaded repo file name**)

    2. Destinations
        {approuter_comfujicargarcomprobantes}_html_repo_host
            "clientId": "sb-92a029a9-2f3e-46aa-8337-e67862dd0342!b76300|html5-apps-repo-uaa!b424"

### html5 Application Repository -> {app}-html5-app-host-service
**app-content**

    3. Service Keys
        comfujicargarcomprobantes-app-content-comfujicargarcomprobantes_html_repo_host-credentials
        "xsappname": "92a029a9-2f3e-46aa-8337-e67862dd0342!b76300|html5-apps-repo-uaa!b424",
> "clientId" 92a029a9-2f3e-46aa-8337-e67862dd0342 = "xsappname" 92a029a9-2f3e-46aa-8337-e67862dd0342 (**destination-service destination key matches html5-app-host-service service key**)        

**Now we know {app} "comfujicargarcomprobantes" is truly the app content we have to match**
