# Ubuntu

## Basic File and Folder Commands

The ls command is used to list files.
```console
ls
```

The 'cd' command is used to change the current working directory. 
```console
cd /var/www
```

The 'mkdir' command is used to make a new directory.
```console
sudo mkdir /var/www/parkingpage
```

The 'chmod' command is used to set or modify a file's permissions.
```console
sudo chmod 775 /var/www
```

The 'chown' command is used to change the file owner.
```console
sudo chown moto /var/www
```

The 'chgrp' command is used to change the group ownership.
```console
sudo chgrp www-data /var/www
```

## Packages

### Update Package Repository
Update the system package list to ensure you get the latest version available in the repository. Run the command below:
```console
sudo apt update
```

### Install Software

Install the Apache2 package by running the following command:
```console
sudo apt install apache2
```

Install the MariaDB package by running the following command:
```console
sudo apt install mariadb-server
```

You can add a -y flag automatically answers yes to any prompts during the installation.

Install the MariaDB package and automatically answers yes to any prompts by running the following command:
```console
sudo apt install mariadb-server -y
```

### Verify Installation

Verify a service is active and running using the following command:
```console
sudo systemctl status mariadb
```