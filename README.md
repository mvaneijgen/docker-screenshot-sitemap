# Docker Puppeteer sitemap screenshot generator

Based on [supalov/docker-puppeteer-dev](https://stackoverflow.com/questions/35093256/how-do-i-pass-an-argument-along-with-docker-compose-up) Github repo

A dockerized [Puppeteer](https://github.com/GoogleChrome/puppeteer) development environment, to work with the [Headless Chrome](https://developers.google.com/web/updates/2017/04/headless-chrome) Node API locally.

## Getting Started

Make sure you have Docker and docker-compose installed and configured so your current user can use both (default with macOS installation). 

Build and run the container it will also start generating screenshots:

Be sure to run the following command from the project root eg `cd `~/YOUR-USER/docker-screenshot-sitemap`

```
SITEMAP=http://domain.com/link/to/sitemap.xml docker-compose up
```

Your images will appear in the `/output/` folder in the root of the project eg `/docker-screenshot-sitemap/output/`

If there is no `SITEMAP` variable being passed it will use the default value in the `docker-compose.yml` file
