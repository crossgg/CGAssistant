# CGAssistant

![](img/logo.png)

[中文说明](READMECN.md)

CGAssistant is a helper for you to play CrossGate with highly automated game experience.

## Warning

This project is only for academic purposes, commercial use is prohibited.

You are prohibited to publish this project elsewhere than GitHub.

However we make no promises to your game accounts and so you have to use this project at your own risk, including taking any damage to your accounts from scripts and binaries.

This project is licensed under MIT License, however if it is otherwise stated before, the latter shall prevail.

## Links

[Source Code](https://github.com/hzqst/CGAssistant)

[Scripts](https://github.com/hzqst/CGAssistantJS)

[Download](https://github.com/hzqst/CGAssistant/releases)

[Wiki](https://github.com/hzqst/CGAssistant/wiki)

## Build Requirement

1. [Visual Studio 2019, with vc142 toolset, with Windows SDK](https://visualstudio.microsoft.com/)

2. [QT 5.15 win32 (x86) for msvc2019, with QtCreator](https://www.qt.io/download)

3. [NodeJS v20.11.1 LTS (32-bit)](https://nodejs.org/)

4. [node-gyp](https://www.npmjs.com/package/node-gyp)

## Build Instruction

Let's assume that you have all requirements installed correctly.

1. Add `Qt5.**\Tools\QtCreator\bin\`, `Qt5.*\5.**\msvc20**\bin\` and `Qt5.**\Tools\QtCreator\bin\jom` (if this folder exists) to your system environment variable "PATH" just like what is mentioned in the snapshot below.

![](img/1.png)

2. Run `init-dep.bat`, wait until all required submodules / dependencies are pulled. (this may takes couple of minutes, depending on your network connection and download speed)

3. Run `build-boost.bat`, wait until all boost static libs are generated. (this may takes couple of minutes, depending on your CPU performance)

4. Run `build-CGAHook.bat`, wait until `CGAHook.dll` is generated under `build` directory.

5. Run `build-qhttp.bat`, wait until `qhttp.dll` generated under `build` directory.

6. Run `build-CGAssiatant.bat`, wait until `CGAssistant.exe` generated under `build` directory.

7. Run `build-nodegyp.bat`, wait until `node_cga.node` generated under `build/Release` directory.

8. Run `windeploy.bat`

Now you have all compiled binaries copied into `build` directory if no error occured.
