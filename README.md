# kysely-sqlite
Dialect to use `node:sqlite` with kysely. Based on the official dialect for `better-sqlite3`.

```sh
npm install kysely-sqlite
```

## Usage
```ts
import { DatabaseSync } from "node:sqlite";
import { Kysely } from "kysely";
import { SqliteDialect } from "kysely-sqlite";

const db = new Kysely({
	dialect: new SqliteDialect({
		database: new DatabaseSync("db.sqlite"),
	}),
});
```
