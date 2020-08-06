## Make new user

Give the username that is already on the your system,

for example. username in home directory is **hdinjos**

before it, login first and use postgres username:

```bash
sudo -iu postgres
```

command to add user to postgresql:

```bash
createuser --interactive --pwprompt
```

than fill **Enter name of role to add** with new username, example **hdinjos**(user already in my system),

enter new password for user created,

enter again to retype password,

and finally, in prompt appear **shall the new role be a superuser?**. Just type **y**

the new user was created



## Make database for new user

Now, make a new database for new user that already created

this very important, because the postgresql must have one database for one user.

You must in terminal like that **[postgres@gNgoding ~]$**, the **gNgoding** is hostname, may different in your system, if quit, can use `sudo -iu postgres` to signin

```bash
createdb -O username dbname
```

the **username** can be replace with new username was already create, and dbname change it with the same the username, example: **create -O hdinjos hdinjos**

type exit to logout