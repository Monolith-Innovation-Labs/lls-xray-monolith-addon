# Lua Language Server X-Ray Monolith add-on
[Addon](https://luals.github.io/wiki/addons/#addon-manager) for [Lua Language Server](https://luals.github.io) that adds support for S.T.A.L.K.E.R lua variant

## Features
### Modules
All `.script` files are threated as a lua module. Global defined in file are accessible on in that file.
![image](https://github.com/user-attachments/assets/0fee8183-f82d-4d2c-bff5-4e3742d81cbb)
![image](https://github.com/user-attachments/assets/f607cd73-9da4-4c72-90da-fc0c1732726f)

### Class
![image](https://github.com/user-attachments/assets/ad805eb8-3c95-4665-8560-77bf2f7ac6d8)
![image](https://github.com/user-attachments/assets/d4259384-d69b-446a-a7da-418c27a1fff1)

## Installation
This add-on is still in its early stages. I don't plan to publish it to the [LLS Add-ons](https://github.com/LuaLS/LLS-Addons) until I finish all the planned features.
### Local installation
1. Download plugin
```
git submodule add https://github.com/Monolith-Innovation-Labs/lls-xray-monolith-addon.git .lua
```
2. create `.luarc.json` file
```json
{
  "runtime": {
     "plugin": "./.lua/xray-plugin.lua",
     "version": "Lua 5.1"
  }
}
```
3. create `.vscode/settings.json` file
```json
{
    "files.associations": {
        "*.script": "lua",
      }
}
```

## Planned Features
- [ ] Definition files for X-Ray Monolith types
