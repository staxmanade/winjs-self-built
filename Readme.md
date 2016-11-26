
# Copy winjs build files
```powershell

cd winjs
grunt storePackage
cd ../winjs-self-built
cp ..\winjs\bin\Microsoft.WinJS* -Recurse .
```