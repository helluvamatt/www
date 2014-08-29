# WWW Deployment

Steps to deploy a new application:

1. Ensure all PHP extensions are installed
2. Provision database (usually in `app/db/create_schema.sql`)
3. `./deploy-app --alias /app --directory app git@github.com:group/www-app.git`
4. `vim app/app/config.json`
5. `systemctl restart httpd.service`

Steps to update an existing application:

**Danger**: This section is subject to change

1. `cd app`
2. `git pull`
