## General Usage

Begin all commands with `inf-wizard` followed by the desired command and any necessary arguments.

Use `inf-wizard --help` to view a summary of available commands.

Use `inf-wizard <command> --help` to view detailed help for a specific command.

## Available Commands



```bash
inf-wizard version
```

Displays the current CLI version.

### Explorer

```bash
inf-wizard explorer getblock
```

Retrieves details of the current block.

```bash
inf-wizard explorer searchblock <blocknumber>
```

Searches for a block by its number.

```bash
inf-wizard explorer checkaddress <address>
```

Displays information about an INF address, including balance, transaction count, and code existence.

```bash
inf-wizard explorer searchtransaction <transactionHash>
```

Searches for transaction details by its hash.

### Staking

```bash
inf-wizard staking stake <privateKey>
```

Stakes INF to the contract using the provided private key.

```bash
inf-wizard staking unstake <privateKey>
```

Unstakes INF from the contract using the provided private key.

```bash
inf-wizard staking get-validators
```

Lists all currently active validators.

### Wallet Management

```bash
inf-wizard wallet createwallet --path <path>
```

Creates a new wallet file at the specified path.

### Node Management



Installs the INF binary.

```bash
inf-wizard node install-inf
```

Dumps the genesis JSON file.

```bash
inf-wizard node get-genesis
```

Initializes INF secrets in the specified data directory.

```bash
inf-wizard node init-secrets --data-dir <directory>
```

Starts the INF node.

```bash
inf-wizard node start-inf-server
```








Happy exploring and interacting with Infinity-Green!