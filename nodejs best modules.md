# Framework should provide

# NPM packages 
### Mysql packages
According to [nodejs mysql] drivers race winner is mysql2 (https://medium.com/epycly/node-js-mysql-driver-benchmarks-2018-86579c402016)
but mysql requires 8 depencies, mariasql 2 (nan, lru-cache) 
* [Mysql](https://www.npmjs.com/package/mysql)  doesnt understrand promises, callback hell yea
* [Mysql2]
* [Knex] depends on mysql or mysql2 but it supports PostgreSQL, MySQL, CockroachDB, MSSQL, SQLite3, Oracle
* [prisma](https://github.com/prisma/prisma) nextjs is using this library, I think its like a good virus that should/will replace existing libs


### CMS's
* [payloadCms](https://github.com/payloadcms/payload) 480MB, early development, dont obey config file, (I needed 3302 port but it starts at 3000), and return notting (yarn run dev) or 404 error (yarn build then yarn serve)
* [keystonejs](keystonejs.com) 683MB
* [strapi](strapi) 832MB for both frontend and backend
* ghost
* [redwoodjs](https://redwoodjs.com/docs/introduction) 1.2GB, requires node v14 ( current node v is 18) trouble working (1 and half day) frontend under docker but api (prismajs) working under port 8911
* [remix.run](https://remix.run/) Using npm and prisma, none feedback/interaction you click, it hangs as then after 1~2 sec (mysql server is not near) loads content.
* [hydrogen](https://shopify.dev/api/hydrogen) shopify's react framework, looks promising, will try


### SERVER SIDE FRAMEWORKS
* express if like a knife, you should carve everything
* nestjs ?

### nodejs fileupload
* [multer] adds 22 packages, works automatically, hard to control name of file.  uses busyboy. 
* [busboy] adds 3 packages, you bind to it


### nodejs requests
* [request](https://www.npmjs.com/package/request) has been depreccated
* https.request is variant
* [axios] has only redirect depency
