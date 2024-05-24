# AZ angular static web app with API
https://learn.microsoft.com/en-us/training/modules/publish-static-web-app-api-preview-url/


### Setup
Because you have the options to choose different frameworks (react, angular, svelte, vue) you first have to decide, which one to use. CDeee into its dir and install its dependencies.

Use the *Bash Console!*
`cd angular-app`
`npm install` this will cause errors because of codelyzer@"^0.0.28" therefore run `npm install --legacy-peer-deps` and ignore the shown vulnerabilities etc.
Run the now with `npm start`

The app is running unter http://localhost:4200/products and shows "Loading data ..." because the API needs to be connected.


#### Install Azure Function Tools
To create the API you need to install Azure Function Tools and also the Azure Function Extension in VSC.

- `npm install -g azure-functions-core-tools@3`
- Install Azure Functions Extension
  
Move up into the root of the whole project.
`cd ..` you are now in **/angular-api-demo** project root, where the API dir is for all frameworks at once:
```
angular-app/  CODE_OF_CONDUCT.md  LICENSE-CODE  react-app-new/  resources/   SETUP.md     vue-app/
api/          LICENSE             react-app/    README.md       SECURITY.md  svelte-app/
```
Now move into the **/api** and run `func start`.

The API is now running and the angular Frontend Webapp can load the data from it. 
