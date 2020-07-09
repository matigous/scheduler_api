# scheduler_api
Scheduler node.js api.

REST API Structure: 

------------------------------------------------------------
Package Manager: yarn
------------------------------------------------------------

Available -> GET LIST

Notifications -> PUT List, GET Update

Schedule -> GET List

Appointments -> POST Create, GET List, DEL Delete

Providers -> GET Index

Sessions -> POST Create

Users -> POST Create, PUT Update

Files (Avatar) -> POST Create

-----------------------------------------------------------

Docker Databases: MySQL, MongoDB, REDIS:ALPINE

-----------------------------------------------------------

Sequelize migration commands:
yarn sequelize db:create // Create DB 
yarn sequelize db:migrate // Migrate DB Structure

-----------------------------------------------------------

Start Server: 
yarn dev (default server) 
yarn queue (queue server for faster async emails send)

-----------------------------------------------------------

