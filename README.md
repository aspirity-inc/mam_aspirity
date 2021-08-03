# Namespace for MAM based projects

## Development

### Local

1. Update NodeJS to LTS
2. Clone [MAM repository](https://github.com/hyoo-ru/mam) and install dependencies via npm or yarn

```bash
git clone https://github.com/hyoo-ru/mam.git ./mam
cd ./mam
npm install
```

3. Clone [this repository](https://github.com/aspirity-ru/mam_aspirity) to `./mam/aspirity`

```bash
git clone https://github.com/aspirity-ru/mam_aspirity.git ./aspirity
```

4. Build the project you want `npm run start aspirity/<project-name>`

5. Run dev server `npm run start`
6. Open url `http://127.0.0.1:9080`
7. Disable cache in devtools
8. Select project in browser

### Gitpod

1. Open [![Gitpod Online Dev Workspace](https://img.shields.io/badge/Gitpod-Online--Dev--Workspace-blue?logo=gitpod)](https://gitpod.io/#https://github.com/hyoo-ru/mam)
2. Install recommended plugins
3. And continue from point 3 in the Local section

### Setup VSCode
- Use MAM directory as root of your project in editor
- [Install VScode intellisense plugin for *.view.tree files](https://marketplace.visualstudio.com/items?itemName=valikov.tree-language-service)
- [Install plugin for *.tree files](https://open-vsx.org/extension/nin-jin/vscode-language-tree)
- [Install .editorconfig plugin](https://open-vsx.org/extension/EditorConfig/EditorConfig)

### How to make VSCode support multiple GIT repositories

1. Create `./mam/.gitmodules` file with similar content. 
```
[submodule "aspirity_restmock"]
    path = aspirity/restmock
    url = git@github.com:aspirity-ru/aspirity_restmock.git
```
2. Edit name, path and link as needed. The file can contain many submodules
