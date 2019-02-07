Remove old version of phonegap
`npm uninstall -g phonegap`
Delete node_modules/ and platforms/ folders

Install correct version of phonegap
`npm install -g phonegap@6.5.1`

Install packages (while located in root of repo)
`npm install`

Need to have version 25 of Android sdk installed
Download https://dl.google.com/android/repository/tools_r25.2.3-windows.zip
Extract into C:\Users\<user>\AppData\Local\Android\Sdk\tools directory, overwrite any files needed
Replace above path with the path to Android tools installation location on your system

Remove any old platform installations
```
phonegap platform remove browser
phonegap platform remove android
```

Reinstall platforms
```
phonegap platform add browser
phonegap platform add android
```

Build platforms
```bash
phonegap build android
# apk is output in platforms/android/build/outputs/apk
phonegap build browser
```

Run/test platforms
```bash
phonegap run android
phonegap run browser
```

