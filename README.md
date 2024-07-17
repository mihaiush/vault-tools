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

## vlookup
Bash lookup client without `vault` binary
```
./vlookup 
vlookup PATH [KEY=value]
Required VAULT envvars:
  VAULT_ADDR
  VAULT_ROLE_ID
  VAULT_SECRET_ID
  VAULT_AUTH_METHOD - vault auth list
```
Tested only with `approle`, most probably will not work with other auth types.

