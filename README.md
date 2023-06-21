# Docker PHP-FPM 8.1 & Nginx 1.24 on Alpine Linux
Based on [this repository](https://github.com/TrafeX/docker-php-nginx), but with some minor tweaks -- namely, the addition of PHP 8.1 extensions for SQLite and SQLite 3.

## Usage

Start the Docker container:

    docker run -p 80:8080 ghcr.io/valoresports/docker-php-nginx

See the PHP info on http://localhost, or the static html page on http://localhost/test.html

Or mount your own code to be served by PHP-FPM & Nginx

    docker run -p 80:8080 -v ~/my-codebase:/var/www/html ghcr.io/valoresports/docker-php-nginx

## Credits

Thanks go to [TrafeX for their original repo](https://github.com/TrafeX/docker-php-nginx).
