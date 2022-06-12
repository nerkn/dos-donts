# Framework should provide

# NPM packages 
### Mysql packages
According to [nodejs mysql] drivers race winner is mysql2 (https://medium.com/epycly/node-js-mysql-driver-benchmarks-2018-86579c402016)
but mysql requires 8 depencies, mariasql 2 (nan, lru-cache) 
* [Mysql](https://www.npmjs.com/package/mysql)  doesnt understrand promises, callback hell yea
* [Mysql2]
* [Knex] depends on mysql or mysql2 but it supports PostgreSQL, MySQL, CockroachDB, MSSQL, SQLite3, Oracle

### CMS's
* [keystonejs](keystonejs.com) 683MB
* [strapi](strapi) 832MB for both frontend and backend
* ghost
* [redwoodjs](https://redwoodjs.com/docs/introduction) 1.2GB, requires node v14 ( currently 18) trouble working (1 and half day) frontend under docker but api (prismajs) working under port 8911


### nodejs fileupload
* [multer] adds 22 packages, works automatically, hard to control name of file.  uses busyboy. 
* [busboy] adds 3 packages, you bind to it


### nodejs requests
* [request](https://www.npmjs.com/package/request) has been depreccated
* https.request is variant
* [axios] has only redirect depency
