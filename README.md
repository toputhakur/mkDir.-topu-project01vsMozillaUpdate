# mkDir.-topu-project01vsMozillaUpdate
How to Stop Permanently Mozilla Update 2021

Post Firefox v89 update, Mozilla has disabled the option to both 1) disable automatic updates and 2) disable check updates
This teeny tiny video shows a permanent fix if you want to disable both the Firefox auto-update feature and auto-check-update feature. 


You can also copy-paste from below.

JSON file mentioned in the video:
filename: "policies.json" (exclude quotes)
Contents: (copy from below to the final brace)
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
