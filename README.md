run `docker build -f Dockerfile.dev .`

take note of the image id created, if you missed it
`docker image ls`

run
bash `docker run -p 3000:3000 -v /app/node_modules -v $(pwd):/app <IMAGEID>`
pwsh `docker run -p 3000:3000 -v /app/node_modules -v ${pwd}:/app <IMAGEID>`
cmd `docker run -p 3000:3000 -v /app/node_modules -v %cd%:/app <IMAGEID>`
