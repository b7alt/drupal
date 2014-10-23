# docker-drupal

Drupal 7.x with SQLite on Nginx, with SSH access for drush, Ubuntu 13.04

## Build

In a clone of this repo:

`docker build -t drupal .`

## Use

This image exposes port 80 for web traffic and port 22 for optional SSH access.

To use:

`docker run -d -p 80 -p 22 -t drupal`

If you don't need SSH access (you usually do to upload libraries and reset premissions on settings.php), just omit `-p 22`
