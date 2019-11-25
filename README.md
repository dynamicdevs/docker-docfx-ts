# Docker Image - DocFx for Typescript

DocFx is a Document generator for Typescript projects

- For Use documentation refer to [DocFx Official Site](https://dotnet.github.io/docfx/tutorial/universalreference/gen_doc_for_js.html).

## Instructions

You can build your document code with the following command:

```sh
docker run --rm --name docfx \
-v path-to-docs-folder:/docfx \
-v path-to-src-if-apply:/src \
    dynamicdevs/docfx-ts:latest
```

### **Important**

- You should map document directory into `/docfx` directory.
- `docfx.json` and `node2docfx.json` files should be in the same directory
- Whether your `src` folder is into directory `/docfx` folder don't map the `src` volume

## Plugins

- Plugins `memberpage`, `rest.operationpage`, `rest.tagpage` are in this image on the `/docfx/plugins` directory
