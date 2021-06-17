# Description
## Publishing a new image
### Build a new version
`docker build ./ -t propertymeld/postgres`
### Tag new version
Replace `13.3` with the appropriate Postgres version
`docker tag propertymeld/postgres propertymeld/postgres:13.3`
### Push to docker
You'll need to be added to Property Meld's Dockerhub team.
`docker push propertymeld/postgres:13.3`