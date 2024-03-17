## SQL injection:

- This occurs when user controlled input is passed to SQL queries. As a result, an attacker can pass in SQL queries to manipulate the outcome of such queries.

* Access, Modify and Delete information in a database when this input is passed into database queries.
  => steal sensitive information such as personal details and credentials.

## Command injection:

- This occurs when user input is passed to system commands. As a result, an attacker is able to execute arbitrary system commands on application servers.

* Execute Arbitrary system commands on a server that would allow an attacker to gain access to users’ systems.
  => steal sensitive data and carry out more attacks against infrastructure linked to the server on which the command is executed.
  For Example:

```
    system($_REQUEST["cmd"]);
```
