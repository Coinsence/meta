
# Update Deployment

- [Servers](#servers)
	- [Dev server](#dev-server)
	- [Preprod server](#test-server-preprod)
	- [Prod server](#community-server-prod)
- [How to update](#how-to-update)
  - [Modules path](#modules-path)
  - [Steps](#steps)

This is a guide of how to upload module updates.

## Servers

### Dev server:

##### Acess:
`ssh username@ip -i pkey`

`pkey`: private key

##### Deployment path:
`/home/ubuntu/dev-coinsence`

##### MySQL configs:
Not yet configured

### Test Server (Preprod):

##### Access:
`ssh username@ip` and type the password.

##### Deployment path:
`/var/www/xcoin-test/htdocs`

##### MySQL configs:
account infos: `/home/xcoin-test/.my.cnf`
PhpMyAdmin: https://test.coinsence.org/phpmyadmin

### Community Server (Prod):

##### Access:
`ssh username@ip` and type the password.

##### Deployment path:
`/var/www/coinsence/htdocs`

##### MySQL configs:
account infos: `/home/coinsence/.my.cnf`
PhpMyAdmin: https://community.coinsence.org/phpmyadmin

## How to update

### Modules path:
- xcoin: `protected/modules/xcoin`
- tasks: `protected/modules/tasks`
- custom_pages: `protected/modules/custom_pages`

### Steps:
1- `cd protected/modules/{your_module}`

2- `git pull` to update the module.

3- resolve whatever git issues you encouter.

4- `rm runtime/cache/ -rf` to actualise the cache (needed for the test server).
