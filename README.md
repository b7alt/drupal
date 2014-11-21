# docker-drupal

Drupal >= 7.34 already installed (admin/test) 
with SQLite on Nginx, APC, with SSH access for drush, Ubuntu 14.04.1 LTS

## Build

In a clone of this repo:

`docker build -t drupal .`

## Use

This image exposes port 80 for web traffic and port 22 for optional SSH access.

To use:

`docker run -d -p 8080:80 -p 2222:22 -t drupal`

If you don't need SSH access (you usually do to upload libraries and reset premissions on settings.php), just omit `-p 22`
