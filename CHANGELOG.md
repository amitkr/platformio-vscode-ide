# Release Notes

## 0.9.0 (2017-12-28)

* Upgraded to PIO Core 3.5.0
* Pre-install PIO Home in pair with PIO Core (resolve issue with "timeout")
* Fixed issue with PIO Core update/upgrade commands (issue [#62](https://github.com/platformio/platformio-vscode-ide/issues/62))

## 0.8.2 (2017-12-02)

* Fixed issue with broken PIO Home and user's Python <2.7.9 (Windows). Automatically install compatible Python

## 0.8.1 (2017-11-29)

* New configuration option: "Update Terminal configuration with patched PATH environment", default is `true`
* Fixed "Expression preceding parentheses of apparent call must have (pointer-to-) function type" for IntelliSense (issue [#54](https://github.com/platformio/platformio-vscode-ide/issues/54))

## 0.8.0 (2017-11-26)

**Requires VSCode 1.18.0 or above**

* Updated PIO Terminal with new VSCode API
* Increased timeout for PIO Home Server

## 0.7.4 (2017-11-03)

* Improved support for non-ASCII locales
* Fixed issue with the missing toolchain includes in `includePath` of IntelliSense

## 0.7.3 (2017-09-09)

* Catch errors when checking PIO Core version (broken PIO Core installation)
* Override LC_ALL only for Darwin platform

## 0.7.2 (2017-09-01)

* Show PIO Home icon on bottom Toolbar even when PIO Project is not opened

## 0.7.1 (2017-09-01)

* Fixed installer issue "Reference Error: atom is not defined" (issue [#38](https://github.com/platformio/platformio-vscode-ide/issues/38))

## 0.7.0 (2017-09-01)

* New in PIO Home:
  - New Project
  - Import Arduino IDE Project
  - Open Project
  - Project Examples
* Migrate to "platformio-node-helpers", a common interface for Node.JS based PlatformIO IDE extensions
* Revert back "Run a task" button on the PIO Toolbar

## 0.6.0 (2017-08-10)

* Integrate new PIO Home 2.0

## 0.5.3 (2017-08-05)

* Ignore broken `node-tar` (3.1.9) package which blocks PIO Core installer

## 0.5.2 (2017-07-27)

* Use dedicated terminal panel per unique PIO Task
* Avoid concurrent "IntelliSense Index Rebuild" processes

## 0.5.1 (2017-07-18)

* Add new Tasks
  - Rebuild C/C++ Project Index
  - Update installed platforms, packages and libraries
  - Upgrade PlatformIO Core
* Use `pio device monitor` command instead of `pio run -t monitor` for "Monitor" task

## 0.5.0 (2017-07-17)

**Requires VSCode 1.13.0 or above**

* Dynamic Tasks (issue [#24](https://github.com/platformio/platformio-vscode-ide/issues/24))
* Custom tasks per project environment based on `platformio.ini` (issue [#16](https://github.com/platformio/platformio-vscode-ide/issues/16))
* Removed "No task is currently running" warning (issue [#26](https://github.com/platformio/platformio-vscode-ide/issues/26))
* Fixed issue with Windows accounts that contain spaces in user name (issue [#27](https://github.com/platformio/platformio-vscode-ide/issues/27))

## 0.4.0 (2017-07-05)

* New `platformio-ide.forceUploadAndMonitor` configuration option which allows to force "Upload and Monitor" task for `platformio-ide.upload` command
* Automatically terminate previous PlatformIO Task before a new (fixes issue with uploading when Serial Monitor is run)

## 0.3.1 (2017-06-28)

* Improved PIO IDE Installer (issue with `virtualenv` and OS temporary directory)
* Added workaround for [Windows command-line string limitation](https://support.microsoft.com/en-us/help/830473/command-prompt-cmd.-exe-command-line-string-limitation)
  (issue [#15](https://github.com/platformio/platformio-vscode-ide/issues/15))

## 0.3.0 (2017-06-05)

* Added default keybindings for the popular commands (Build, Upload, Open Serial Monitor, Initialize New Project, Run Other Tasks)
* Automatically close Serial Monitor before uploading
* Synchronize Installer with the latest version from PIO IDE for Atom
* Don't show PlatformIO Toolbar in non-PlatformIO projects (issue [#6](https://github.com/platformio/platformio-vscode-ide/issues/6))
* Don't replace default terminal with PlatformIO (issue [#9](https://github.com/platformio/platformio-vscode-ide/issues/9))
* Fixed issue with PIO Terminal and Windows PowerShell (issue [#10](https://github.com/platformio/platformio-vscode-ide/issues/10))
* Other improvements and bugfixes

## 0.2.0 (2017-05-29)

* PlatformIO Toolbar in Status Bar (Build, Upload, Clean, Run Tasks, New Project, Serial Monitor, and Terminal)
* Improved auto installer for PIO Core
* Improved C/C++ Code Completion

## 0.1.0 (2017-05-28)

* Initial release
