---
cssclasses:
  - datacore-no-padding
  - datacore-no-border
  - datacore-hide-header
---

```datacorejsx
const activeFile = dc.resolvePath("CARD SCANNER") || "_RESOURCES/DATACORE/_DONE/CARD SCANNER/CARD SCANNER.md";
const folderPath = activeFile.substring(0, activeFile.lastIndexOf('/'));

const { View } = await dc.require(folderPath + "/src/index.jsx");
return await View({ folderPath, dc });
```
