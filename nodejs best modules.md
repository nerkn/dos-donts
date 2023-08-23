# Framework should provide

#Generic libs
[@lukeed/ms] library to convert time to human format like 1 minute, 1 day



# NPM packages 
### Mysql packages
According to [nodejs mysql] drivers race winner is mysql2 (https://medium.com/epycly/node-js-mysql-driver-benchmarks-2018-86579c402016)
but mysql requires 8 depencies, mariasql 2 (nan, lru-cache) 
* [Mysql](https://www.npmjs.com/package/mysql)  doesnt understrand promises, callback hell yea
* [Mysql2]
* [Knex] depends on mysql or mysql2 but it supports PostgreSQL, MySQL, CockroachDB, MSSQL, SQLite3, Oracle
* [prisma](https://github.com/prisma/prisma) nextjs is using this library, 
* [Drizzle Orm](https://orm.drizzle.team/docs/quick-start) with Mysql there are so many errors with migration, pushing changes (int 11 always replaced by int so tables get truncated). I opened a bug report regarding full join, they replied "dont use full join" . Its wonderful to have types from datatable tables (type ImageType = InferModel<typeof images, "insert">; ) 
* [Typeorm]  


### CMS's
* [payloadCms](https://github.com/payloadcms/payload) 480MB, early development, dont obey config file, (I needed 3302 port but it starts at 3000), and return notting (yarn run dev) or 404 error (yarn build then yarn serve)
* [keystonejs](keystonejs.com) 683MB
* [strapi](strapi) 832MB for both frontend and backend
* ghost
* [redwoodjs](https://redwoodjs.com/docs/introduction) 1.2GB, requires node v14 ( current node v is 18) trouble working (1 and half day) frontend under docker but api (prismajs) working under port 8911
* [remix.run](https://remix.run/) Using npm and prisma, none feedback/interaction you click, it hangs as then after 1~2 sec (mysql server is not near) loads content.
* [hydrogen](https://shopify.dev/api/hydrogen) shopify's react framework, looks promising, will try
* 


### SERVER SIDE FRAMEWORKS
* express if like a knife, you should carve everything
* fastify I needed to replace modules' route to another place, in express it was so much easy but fastify dont support route nesting, I read a lot about speed though.
* nestjs After getting used to modules logic, it's like normal framework, I like services logic, light controllers
* nextjs, Its not production ready, pages/app folder is different, next-auth documentation is so confusing, they are like catched a big hype wave and with the help of community trying to find solutions. I'd highly suggest nestjs + react. I think concepts they bring braking more bones than solutions. But viewpoint of a person who has php background I love ssr.

### nodejs fileupload
* [multer] adds 22 packages, works automatically, hard to control name of file.  uses busyboy. 
* [busboy] adds 3 packages, you bind to it


### nodejs requests
* [request](https://www.npmjs.com/package/request) has been depreccated
* https.request is variant
* [axios] has only redirect depency

### auth modules
[next-auth] 

### Docker
* [lazyDocker](https://github.com/jesseduffield/lazydocker) easy way to see running pods in docker-compose
*  Start Project docker
When starting projects I dont want to install anything, so I spin up docker container and inside I start
```
docker run -v $(pwd)/customerReports:/app -w /app -p:5055:5055 -it  node bash
```

