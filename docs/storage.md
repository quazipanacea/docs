# File System

Quazipanacea stores everything directly on the file system.

Currently, there are two location Quazipanacea reads and writes from:

## config

Configuration at `"${XDG_CONFIG_HOME:-$HOME/.config}/quazipanacea/server.json"

```json
{
  "documentsDir": "~/Documents/Quazipanacea"
}
```

## documents

Documents located at `config.documentsDir`. It has the following subdirectories:

```txt
- `single`
- `coupled`
```

- This is the _gold_ level of hierarchy. Silver and bronze have other subcategories
- Of these types, there are also different levels (primary source and secondary/tertiary source)
