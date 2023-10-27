## phase2-ungraded-challenge-10

### Migration 

```bash
migrate create -ext sql -dir migrations create_table_users
```

```bash
migrate create -ext sql -dir migrations create_table_profiles
```

```bash
migrate create -ext sql -dir migrations add_users_column_role
```

### Execute

```bash
migrate -database "postgres://postgres:@localhost/phase2-ngc-10?sslmode=disable" -path migrations up
```
