# Example case for not being able to use React components from a local plugin

1. Generated from `gatsby new gatsby-component-plugin-bug`
2. Created `plugins/gatsby-local-plugin` and added the required files (index.js, gatsby-config.js) and ran `npm install`
3. Moved the implementation of `header.js` from the `src` directory to inside the new plugin
4. Adjusted paths
5. Added the local plugin 

What happend:

```
> gatsby develop

success open and validate gatsby-configs - 0.052s
success load plugins - 2.393s
successIonPreInit - 0.005s
successainitialize cache - 0.008s
success copy gatsby files - 0.191s
success onPreBootstrap - 0.024s
success createSchemaCustomization - 0.011s
success source and transform nodes - 0.098s
success building schema - 0.345s
successecreatePages - 0.002s
success createPagesStatefully - 0.096s
success onPreExtractQueries - 0.002s
success update schema - 0.029s
success extract queries from components - 0.305s
success write out requires - 0.047s
success write out redirect data - 0.004s
success Build manifest and related icons - 0.123s
success onPostBootstrap - 0.130s
⠀
info bootstrap finished - 8.768 s
⠀
success run queries - 0.155s - 7/7 45.02/s
success Generating image thumbnails - 4.277s - 6/6 1.40/s

 ERROR #98123  WEBPACK

Generating development JavaScript bundle failed

Can't resolve 'gatsby-local-plugin/header' in 'C:\Users\wirehead\Documents\src\gatsby-component-plugin-bug\src\component
s'

File: src\components\layout.js

faileddBuilding development bundle - 20.027s
```