# Make Easy To Learn Postgre Sql Database From Zero To Hero

## install on your system
### arch linux => manjaro
```
sudo pacman -S postgresql
```
In the other linux distributions, this command may be different

### check the version
```
postgres --version
```

### login with postgres user
```
sudo -iu postgres
```
enter password for user root

### initial data directory
in firstly installing postgre, data directory not yet binded.
so,manually set data directory in your system
```
initdb --locale en_US.UTF-8 -D /var/lib/postgres/data
```
### active the service postgresql in system
before it, if you still login with user postgres. logout it
and active the service
```
sudo systemctl start postgresql
```
### set auto run on booting (once if the first installing)
```
sudo systemctl enable postgresql
```

### ready to run
```
psql postgres
```
the postgres is user to enter database system
you can make the other user for database posgre system

### what next?
1. [make new user for database system](https://github.com/hdinjos/initial-postgres/tree/master/add-new-user)
2. [enter new user](https://github.com/hdinjos/initial-postgres/tree/master/enter-new-user)
3. [database](https://github.com/hdinjos/initial-postgres/tree/master/database)
4. [table](https://github.com/hdinjos/initial-postgres/tree/master/table)
5. [constraints](https://github.com/hdinjos/initial-postgres/tree/master/constrain)
