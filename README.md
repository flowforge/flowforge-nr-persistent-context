# @flowforge/nr-auth

A Node-RED Context Plugin for the FlowForge platform.

This plugin provides persistent context for a Node-RED instance
on the FlowForge platform.

### Configuration

```js
contextStorage: {
    file: {
        module: require("@flowforge/nr-context"),
        config: {
            projectID: process.env['FORGE_PROJECT_ID'],
            baseURL: process.env['FORGE_STORAGE_URL'],
            token: process.env['FORGE_STORAGE_TOKEN']
        }
    }
}
```

 - `projectID` - is the UUID of the project
 - `baseURL` - the root URL for the FlowForge Storage API
 - `token` - authentication token