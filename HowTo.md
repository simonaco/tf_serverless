## What do we need
1. Azure CLI
2. Docker
3. Azure Functions Core Tools

4. Create a Python 3.6.* VirtualEnv and activate it
5. From `AzTFServerless` folder, run `pip -r requirements.txt --ignore-installed`

6. Check out the function locally by running `func host start`. This spins up a server. You can use the convenient `upload.html` file to upload an image to see the results from our ML model.

7. Complete instructions for functions deployment here: https://docs.microsoft.com/en-us/azure/azure-functions/functions-create-first-function-python
- Resource Group Creation
- Storage Account Creation
- Create Linux Function App (mine is called `tfserverless`)

8. Deploy the Function App.

Depending on your system version of Python you might not be able to use both the VirtualEnv and the Azure CLI at the same time. Deploy instead by executing a build in a Docker container:

```
func azure functionapp publish tfserverless --build-native-deps
```

9. Update the action in the handy form upload page `upload.html` provided to point to the new URL including the function key param.