# specifi

## Running project on local
First of all create new folder, and clone this repo inside of it. After that clone the others.

`git clone git@github.com:h22k/specifi-backend.git`

`git clone git@github.com:h22k/specifi-front.git`

After these operations, your folder structure should be:

- Main folder - you have created
  - specifi-docker
  - specifi-backend
  - specifi-front

when you are sure that everything has done successfully, 
make sure that the necessary ports (**8000, 5173, 5432**) are available.

Laravel is running: 8000

Vue is running: 5173

PgSql is running: 5432


Go inside specifi-docker folder then run

`docker compose up -d`

after that, the last step is when you are inside of specifi-docker you should run 

`docker compose exec backend bash` then run `php artisan migrate --seed`

and finally you ready to go, visit localhost:5173 on your browser.