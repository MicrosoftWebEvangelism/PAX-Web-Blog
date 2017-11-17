## Local Setup - Docker Compose

It is higly recommended that you run this project using Docker to keep it from interfering with any other Ruby or Jekyll projects you may have. Once you have Docker installed, run

```bash
$> docker-compose up
```

That will spin up the Docker VM instance and run the site for you.

If you want to jump into the command line within the Docker VM, run

```bash
$> docker-compose run jekyll bash
```

## Local Setup - Raw

Navigate to the root directory and run the following command:

```bash
$> bin/setup
```

## Local Testing

To test your stuff locally, you’ll need to run the following:

```bash
$> bundle exec jekyll serve
```

If you are running under Docker, you will need to point your broser at the correct IP for the VM.

## Local Building

To build your site, run

```bash
$> bundle exec jekyll build --incremental
```

## Deployment

To deploy to Github Pages

```bash
$> bin/deploy
```

That will push the built site to the `gh-pages` branch.