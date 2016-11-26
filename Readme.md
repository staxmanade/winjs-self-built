
Since WinJS is being sun-setted, I'm using this as a place to store a custom build of WinJS that has bug-fixes I've added and can include WinJS into a project using JSPM.


# Dev Notes:

1. setup the following folder structure

```

./winjs/ <-- this maps to https://github.com/winjs/winjs/
./winjs-self-built <-- this maps to https://github.com/staxmanade/winjs-self-built

```

```powershell

cd winjs
grunt storePackage
cd ../winjs-self-built
cp ..\winjs\bin\Microsoft.WinJS* -Recurse .
# git commit changed files
npm version patch
npm publish
```
