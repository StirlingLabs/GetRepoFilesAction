# 📦 Get Repo Files Action

> Get a few files from the current repo, without checking everything out

## ⭐ Features

- Get files quickly.

## 🚀 Quickstart

```yaml
      # Store this asset in 'gh-storage' branch.
      - name: Get Files
        uses: StirlingLabs/GetRepoFilesAction@23.04.0
        with:
          files: |
            icon.png
            README.md
          filesJson: |
            { "title.jpg": "banner.jpg", 
              "src/header.h": "header.h"
              }
```

## Parameters

|Name|Function|
|-|-|
|files|List of files to download, 1 per line|
|jsonFiles|JSON list of files to get and rename, in the format  `{"repo_name": "local_name", ...}` |