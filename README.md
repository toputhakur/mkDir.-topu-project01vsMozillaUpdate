# mkDir.-topu-project01vsMozillaUpdate
How to Stop Permanently Mozilla Update 2021

Post Firefox v89 update, Mozilla has disabled the option to both 1) disable automatic updates and 2) disable check updates
This teeny tiny video shows a permanent fix if you want to disable both the Firefox auto-update feature and auto-check-update feature. 

You can also copy-paste from below.

01.make a directory in installation folder name as "Distribution"
02.creat a file name: "policies.json" (exclude quotes) in this folder with notepade++
03.copy from below to the final bracet
04.save

{
  "policies": {
    "DisableAppUpdate": true,
    "DisableFirefoxStudies": true,
    "DisablePocket": true,
    "DisableSystemAddonUpdate": true,
    "DisableTelemetry": true,
    "ExtensionUpdate": false,
    "Preferences": {
      "security.ssl.errorReporting.enabled": false
    }
  }
}
