# Description
This is a custome image based of CircleCI's postgres. We are adjusting some of the config in `postgresql.conf` to avoid running into errors when running many tests in parallel.
## Publishing a new image
### Build a new version
`docker build ./ -t propertymeld/postgres`
### Tag new version
Replace `13.3` with the appropriate Postgres version

`docker tag propertymeld/postgres propertymeld/postgres:13.3`
### Push to docker
You'll need to be added to Property Meld's Dockerhub team.

`docker push propertymeld/postgres:13.3`