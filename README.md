# Docker Puppeteer sitemap screenshot generator

Based on [supalov/docker-puppeteer-dev](https://stackoverflow.com/questions/35093256/how-do-i-pass-an-argument-along-with-docker-compose-up) Github repo

A dockerized [Puppeteer](https://github.com/GoogleChrome/puppeteer) development environment, to work with the [Headless Chrome](https://developers.google.com/web/updates/2017/04/headless-chrome) Node API locally.

## Getting Started

Make sure you have Docker and docker-compose installed and configured so your current user can use both (default with macOS installation).

Build and run the container it will also start generating screenshot:

```
SITEMAP=http://domain.com/link/to/sitemap.xml docker-compose up
```

Your images will appear in the `/output/` folder

If there is no `SITEMAP` variable being passed it will use the default value in the `docker-compose.yml` file
