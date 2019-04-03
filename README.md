## HTML Report Workaround

1. From the Jenkins home screen navigate to `Manage Jenkins > Script Console` and type in the following command:

```
 System.setProperty("hudson.model.DirectoryBrowserSupport.CSP", "")
``` 

2. Then press `Run`.
3. If you see the output as `Result:` below the Result header, then it has run successfully.
4. You'll need to `Commit` and `Push` again so that another build creates another HTML report before you can see one generated successfully.

## Allure report

From the command line:

`allure serve <xml or json file directory>`

