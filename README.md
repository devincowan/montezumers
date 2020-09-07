# Forked From [Bedrock](https://roots.io/bedrock/)

## Requirements

* PHP >= 5.6
* Composer - [Install](https://getcomposer.org/doc/00-intro.md#installation-linux-unix-osx)

## Installation
1. Clone the repo (ex: into /var/www/)

2. Update environment variables in `.env`  file:
  * `DB_NAME` - Database name
  * `DB_USER` - Database user
  * `DB_PASSWORD` - Database password
  * `DB_HOST` - Database host
  * `WP_ENV` - Set to environment (`development`, `staging`, `production`)
  * `WP_HOME` - Full URL to WordPress home (http://example.com)
  * `WP_SITEURL` - Full URL to WordPress including subdirectory (http://example.com/wp)
  * `AUTH_KEY`, `SECURE_AUTH_KEY`, `LOGGED_IN_KEY`, `NONCE_KEY`, `AUTH_SALT`, `SECURE_AUTH_SALT`, `LOGGED_IN_SALT`, `NONCE_SALT`

 

  Cut and paste salts from the [Roots WordPress Salt Generator][roots-wp-salt].

3. Add theme(s) in `web/wp-config/themes` as you would for a normal WordPress site.

4. Set your site vhost document root to `/path/to/site/web/` (`/path/to/site/current/web/` if using deploys)

5. Access WP admin at `http://example.com/wp/wp-admin`

## Deploys

`composer install` must be run as part of the deploy process.

## Documentation

Bedrock documentation is available at [https://roots.io/bedrock/docs/](https://roots.io/bedrock/docs/).
[roots-wp-salt]:https://roots.io/salts.html
[wp-cli-dotenv]:https://github.com/aaemnnosttv/wp-cli-dotenv-command
