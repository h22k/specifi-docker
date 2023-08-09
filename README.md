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

------
## if there is no .env file inside backend
`docker compose exec backend bash` then run `cp .env.example .env`

--------

`docker compose exec backend bash` then run `php artisan migrate --seed`

and finally you ready to go, visit localhost:5173 on your browser.

| Element | is done |
|---------|---------|
|Ability for users to create, update, and delete tasks.      | 50%     |
|Task categories (e.g., personal, work, etc.) with the ability to assign tasks to categories  | 50%     |
|Task status (e.g., todo, in progress, done) with the ability to update the status of tasks    | 50%     |
|User interface to view and filter tasks by category and status      | 0%      |
|Ability to search for tasks by name or description       | 100%    |
|Implement RESTful API endpoints for task management operations.         | 50%     |
|Use Vue.js for the frontend implementation and interact with the backend APIs.         | 100%    |
|Implement appropriate error handling and display error messages to users when necessary.         | 100%    |
|Apply best practices in code organisation, maintainability, and security.         | 50%     |

