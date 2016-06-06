# Mautic Install Shell Script for Cloud9

This is simple shell script to install Mautic on Cloud9

Currently, this script downloads 1.4.1.

## STEP 1: Create a worksplace

- Create a workspace on Cloud9 using Apache+MySQL+PHP template

## STEP 2: Initiate MySQL

Copy and paste the following texts and paste onto the Cloud9 terminal window to start MySQL and create user and password.

```
mysql-ctl start
mysql-ctl cli
CREATE USER 'mautic'@'127.0.0.1' IDENTIFIED BY 'mautic';
GRANT ALL PRIVILEGES ON *.* TO 'mautic'@'127.0.0.1' WITH GRANT OPTION;
FLUSH PRIVILEGES;
exit;

```

## STEP 3: Download & Initialte the file

```
wget https://github.com/katzueno/mautic-install-shell/blob/master/install-mautic-cloud9.bash
sh install-mautic-cloud9.sh

```

## STEP 4: Launch your browser to proceed to browser installation

- Click "Preview" to open the browser
- Proceed to installation

Use the following MySQL information to install

Type           | Content
---------------|-----
MySQL Address  | 127.0.0.1
MySQL Username | mautic
MySQL Password | mautic
Database Name  | c9

Enter the rest of the required information as you wish.


# Credit

@katzueno (concret5 Japan, Inc.)

concrete5 Japan, Inc. is helping various company's concrete5 & Mautic project. Please feel free to contact us at any time for your project needs. We can work internationally.

https://concrete5.co.jp/
