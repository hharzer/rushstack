[Home](./index) &gt; [@microsoft/rush-lib](./rush-lib.md) &gt; [RushConfiguration](./rush-lib.rushconfiguration.md) &gt; [tempShrinkwrapFilename](./rush-lib.rushconfiguration.tempshrinkwrapfilename.md)

# RushConfiguration.tempShrinkwrapFilename property

The full path of the temporary shrinkwrap file that is used during "rush install". This file may get rewritten by the package manager during installation.

**Signature:**
```javascript
tempShrinkwrapFilename: string
```

## Remarks

This property merely reports the filename; the file itself may not actually exist. Example: "C:\\MyRepo\\common\\temp\\npm-shrinkwrap.json" or "C:\\MyRepo\\common\\temp\\shrinkwrap.yaml"