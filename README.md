# References

- https://www.udemy.com/course/api-completa-com-adonisjs-5-typescript-e-tdd/
- https://docs.adonisjs.com/cookbooks/testing-adonisjs-apps

- https://medium.com/@piyumimdasanayaka/json-web-token-jwt-vs-opaque-token-984791a3e715
- https://github.com/adonisjs/core/discussions/1365
- https://docs.adonisjs.com/guides/auth/social

# Comandos
- $ node ace --help
- $ node ace make:controller --help
- $ node ace make:controller User
- $ node ace configure @adonisjs/lucid
- $ node ace make:model User
- $ node ace make:migration users
- $ node ace make:exception BadRequest
- $ node ace make:validator CreateUser
- $ node ace make:validator UpdateUser
- $ node ace make:model LinkToken -m 
- $ node ace make:validator ForgotPassword
- $ node ace make:validator ResetPassword
- $ node ace make:exception TokenExpired
- $ node ace make:controller Session
- $ node ace configure @adonisjs/auth
- $ node ace:make controller Group
- $ node ace:make model Group -m 


# DataBase 
- The package has been configured successfully. The database configuration stored inside config/database.ts file relies on the following environment variables and hence we recommend validating them.

- Open the env.ts file and paste the following code inside the Env.rules object.
   - DB_CONNECTION: Env.schema.string(),

## Variables for the MYSQL driver

    MYSQL_HOST: Env.schema.string({ format: 'host' }),
    MYSQL_PORT: Env.schema.number(),
    MYSQL_USER: Env.schema.string(),
    MYSQL_PASSWORD: Env.schema.string.optional(),
    MYSQL_DB_NAME: Env.schema.string(),

    * The MYSQL_HOST should always be present and formatted as a valid host.
    * The MYSQL_PORT should always be present and a valid number.
    * The MYSQL_USER and MYSQL_PASSWORD are required to authenticate with the database server. The password is marked as optional since many local database servers are configured to work without passwords.
    * The MYSQL_DB_NAME is the database name you want to connect with.

## Variables for the PostgreSQL driver

    PG_HOST: Env.schema.string({ format: 'host' }),
    PG_PORT: Env.schema.number(),
    PG_USER: Env.schema.string(),
    PG_PASSWORD: Env.schema.string.optional(),
    PG_DB_NAME: Env.schema.string(),

## Variables for the MSSQL driver

    MSSQL_SERVER: Env.schema.string({ format: 'host' }),
    MSSQL_PORT: Env.schema.number(),
    MSSQL_USER: Env.schema.string(),
    MSSQL_PASSWORD: Env.schema.string.optional(),
    MSSQL_DB_NAME: Env.schema.string(),

## Variables for the OracleDB driver

    ORACLE_HOST: Env.schema.string({ format: 'host' }),
    ORACLE_PORT: Env.schema.number(),
    ORACLE_USER: Env.schema.string(),
    ORACLE_PASSWORD: Env.schema.string.optional(),
    ORACLE_DB_NAME: Env.schema.string(),
CREATE: ace-manifest.json file
