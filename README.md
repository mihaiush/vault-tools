# vault-tools
Hashicorp Vault Tools

## vcp
Recursive copy between two vault paths
```
./vcp 
vcp [-x|--execute] [-v|--verbose] SRC DTS
  -x, copy, otherwise dry-run
  -v, show vault data
```
If `SRC` ends with `/` copies all paths under `SRC` under `DST`. Without `/` copies `SRC` under `DST`.
