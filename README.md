# scheduler_api
Scheduler node.js api.

REST API Structure: 

------------------------------------------------------------
Package Manager: yarn
------------------------------------------------------------

Available -> GET LIST

Notifications (Mongoose integration) -> PUT List, GET Update

Schedule -> GET List

Appointments -> POST Create, GET List, DEL Delete (nodemailer send)

Providers -> GET Index

Sessions (JWT - JSONWEBTOKEN) -> POST Create

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
yarn dev (default server) // 
yarn queue (Redis queue server for faster async emails send)

-----------------------------------------------------------

ENVIRONMENT VARIABLES EXAMPLE (.env)

<h5>App</h5>

APP_URL=http://localhost:3333
NODE_ENV=development

<h5>Auth</h5>

APP_SECRET=anything

<h5>Database</h5>

DB_HOST= ***
DB_USER= ***
DB_PASS= ***
DB_NAME= ***

<h5>Mongo</h5>

MONGO_URL= ***

<h5>Redis</h5>

REDIS_HOST=127.0.0.1
REDIS_PORT=6379

<h5>Mail</h5>

MAIL_HOST= ***
MAIL_PORT= ***
MAIL_USER= ***
MAIL_PASS= ***

<h5>Sentry</h5>

SENTRY_DSN= ***



