#  How to install postgres using docker ?
## - Step 1 => pull the docker latest image
   `docker pull postgres`

## Step 2 => Run the docker run command
  ex
  
  `docker run --name <Name of your image> -d 
               -e POSTGRES_PASSWORD=<your password>
               -p 5432:5432
               - v D:/postgres:/var/lib/postgresql/data postgres`

  --name = Any name of image\
   -d    = it will run docker in bg and gives id\
   -e    = environment variable\
   -p    = Port mapping\
   -v    = data stored or copied from virtual to local storage\


   `docker run --name mypostgres -e POSTGRES_PASSWORD=mypassword -d -p 5432:5432 postgres
`


## How to start?

`docker start <image name>`


