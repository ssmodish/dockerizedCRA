run `docker build -f Dockerfile.dev -t <(you pick the)IMAGENAME> .`

run
bash `docker run -p 3000:3000 -v $(pwd):/app -v /app/node_modules <IMAGENAME>`
pwsh `docker run -p 3000:3000 -v /app/node_modules -v ${pwd}:/app <IMAGENAME>`
cmd `docker run -p 3000:3000 -v /app/node_modules -v %cd%:/app <IMAGENAME>`
