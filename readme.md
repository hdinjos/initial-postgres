# make easy to learn postgre sql database from zero to hero

## install on your system
### arch linux => manjaro
`sudo pacman -S postgresql`

### check the version
`postgres --version`

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
`sudo systemctl enable postgresql`
