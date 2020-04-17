[![Netlify Status](https://api.netlify.com/api/v1/badges/db6c835f-87e3-47c4-8f4d-53b4af3c6be8/deploy-status)](https://app.netlify.com/sites/brooklynrail/deploys)

---

# The Brooklyn Rail
https://brooklynrail.org


## Install

1. [Install Hugo.](https://gohugo.io/getting-started/quick-start/#step-1-install-hugo)
1. Start the server.

   ```sh
   hugo server
   ```

## Importing content

The repository already contains a subset of the articles under `content/`, but if you want modify [the import script](import.js) to bring in more data:

1. Install Node.js.
1. Start the database from [the main site](https://github.com/brooklynrail/brooklynrail) directory.

   ```sh
   docker-compose up db
   ```

1. From this directory, run the import.

   ```sh
   npm install
   node import.js
   ```

You should see directories and files written under `content/`.