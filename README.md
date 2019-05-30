# SQLInjection

This is a little demonstration of a SQL injection in a simple login application. In our example, a database as been provisionned with an admin user. Their credentials are:

> username: admin  
> password: admin123

In theory it should only be possible to login in the application using this credential, but if the application is not safely programmed, it is possible to penetrate in the system as an admin user without knowing the admin password.

Once you have played a bit with the login application and tried to used valid and invalid credential, use the following values

> username: admin  
> password: unknown' or '1'='1

All the SQL statements with the password attempts will be printed to the console if using the run.sh file.

## Instruction to run the demo

1. clone the repository

2. run the command `npm install` in the directory of the repository

3. run the run.sh file `./run.sh` OR for windows users you can simply run `node app.js`

4. go to https://localhost:3000