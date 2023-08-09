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
          files_json: |
            { "title.jpg": "banner.jpg", 
              "src/header.h": "header.h"
              }
```

## Inputs
|Name|Function|
|-|-|
|files|List of files to download, 1 per line|
|files_json|List of files to get and rename, in JSON format: `{"repo_name": "local_name", ...}` |

## Outputs
|Name|Function|
|-|-|
|downloaded|List of files downloaded, 1 per line|
|downloaded_json|JSON array of files downloaded, i.e. `[ "file1.ext", "file2.ext" ... ]` |