# demo1

Local plugin-manager demo, version 0.1.0.

Edit `dist/index.js` directly; there is no build step. `plugin.json` holds the
plugin ID and version. This is a package fixture, not a Tilr runtime plugin.

From the plugin-manager directory:

```sh
./pm install '/Users/dan/projects/tilr/temp-plugin-manager/demo-plugins/demo1' --ref v0.1.0
# After editing this repository:
./pm commit '/Users/dan/projects/tilr/temp-plugin-manager/demo-plugins/demo1' 0.1.1
./pm update demo1 --ref v0.1.1
./pm rollback demo1
```

To register with a running catalog:

```sh
./pm register '/Users/dan/projects/tilr/temp-plugin-manager/demo-plugins/demo1' --ref v0.1.0
```

No remote is configured. If Git identity was missing, the scaffold configured
Plugin Demo <demo@example.invalid> locally in this repository only.
