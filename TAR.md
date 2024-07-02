# tar.gz

## 1. compressed file

### Command

```sh
tar -czvf archive-name.tar.gz dir_name
```
Parameters

    c: creates a new archive.
    z: compresses the archive with gzip.
    v: displays the progress in the terminal (optional but useful to see the process).
    f: specifies the name of the archive file to be created.

## 2. extract the contents

### Command

```sh
tar -xzvf archive-name.tar.gz -C dir_name
```
Parameters

    x: extracts files from the archive.
    z: decompresses the gzip archive, suitable for .tar.gz files.
    v: displays the progress in the terminal (optional).
    f: specifies the name of the archive file to be extracted.
    -C uploads: indicates that the contents should be extracted into the uploads directory.
