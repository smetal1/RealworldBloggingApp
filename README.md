
### RealWorld Blogging App

### Technology Stack and other details
1. Rocket - framework
2. Diesel - ORM

### Step 1: Import DB 
# Install or run postgres DB using docker and use the following commands to seed the data
```sh
psql -f init.sql
cargo install diesel_cli --no-default-features --features "postgres"
diesel migration run
```
### Run
```sh
cargo run
```
### Test
For testing execute the following command
```sh
cargo test
```

### NOTE:
To configure DB related environment variables use .env file present in the base directory
