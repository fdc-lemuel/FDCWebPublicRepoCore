## FDCWebPublicRepoCore
This is a raw cakephp2 with php8 environment usable for trainings

## To get started 
Install docker from their official website https://www.docker.com/
Open folder inside terminal/command prompt
Type and run
```
    docker-compose up -d
```
then just type http://localhost/ the browser

## Your database configuration file is NOT present. (Warning)
Rename the file database.php.default to database.php which is located inside workspace/cakephp/app/config/
configure the database.php file
```
    'login' => 'root',
    'password' => 'cde3bgt5_root',
    'database' => 'database_name', // your database name
```

## Logging in phpmyadmin
```
    'username' => 'root',
    'password' => 'cde3bgt5_root',
```

## Please change the value of 'Security.salt' or 'Security.cipherSeed' (Error)
Edit the file inside workspace/cakephp/app/config/core.php
```
	Configure::write('Security.salt', 'DYhG93b0qyJfIxfs2guVoUubWwvniR2G0FgaC9mi'); // replace this string with a random string

	Configure::write('Security.cipherSeed', '76859309657453542496749683645'); // replace this numbers with a random numeric (digits only)
```
