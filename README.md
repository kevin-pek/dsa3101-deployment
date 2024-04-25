# DSA3101 Manpower Optimisation for MFLG

👋 Hello! This is the deployment repo for our group's application stack. The frontend and backend repos are added as submodules to this repository, tagged to a commit hash that is stable and working.

For more detailed information on the frontend and backend repos, please click on their respective folders!

## Prerequisites

The entire application stack runs on docker, so please make sure you have Docker installed.

## Getting Started

To get started clone this repository, navigate to into the directory and run the following commands:

```sh
git submodule init    # registers the frontend and backend repos as submodules
git submodule update  # pulls the submodule repos
docker compose up -d  # run the entire stack (MySQL, Flask API, React App) in detached mode
```

Once all containers are running the frontend app should now be accessible on port 3000. See `docker-compose.yml` for the port mappings for each service. Alternatively, you can also clone the frontend and backend repos separately and run them manually. See their respective repos for more information.

Should you wish to make any changes in the frontend/backend repositories, you can edit them within the `frontend` and `backend` servers and push/pull any changes within this repo.
