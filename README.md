Boilerplate to create a cumulocity ui plugin

- Get the plugin boilerplate here: https://bitbucket.org/m2m/cumulocity-ui-plugin
- Run *npm install*
- Configure the *cumulocity.json* for application (Select an application name unique in your tenant)
- Register application: *grunt appRegister*
- Configure the *cumulocity.json* for plugin (optional)
- Register plugin: *grunt pluginRegister:<pluginName>* or *grunt pluginRegisterAll*
- Edit the application *cumulocity.json* manifest to include the newly created plugin as an import.
- Re register the application: *grunt appRegister*
- Run local server: *grunt server*
- Open in browser: *http://localhost:8000/apps/<appname>/index.html*
- Code your plugin. Iterate.
- Build your plugin: *grunt build*
- Make sure to re-register if you make changes to manifests: *grunt appRegister*, *grunt pluginRegisterAll*