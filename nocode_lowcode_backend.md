Backend means,
1. connecting db's ( it can be paid services, selfhosted sql-nosql or, file system),
1. authentication (it should handle and track user registration, login )
1. authorization (it should provide roles for users)
1. crud/graphql (how we'll reach db and how well maniplate data)
1. Multi-tenant (can seperate different projects)

PocketBase : one file backend written on go





|Platform|DBs|Auth|Roles|Data Access|MultiTenant|
|--------|---|--|--|--|--|
|<a href="https://www.PocketBase.io/" target='PocketBase'>PocketBase</a>|Sqlite|Provides|?|REST-ish API|?|
|<a href="https://www.appflowy.io/" target='appflowy'>appflowy</a>|?|||||
|<a href="https://nocodb.com/" target='nocodb'>nocodb</a>|All sql DBs||||apis have org and projectname|
|<a href="https://appsmith.com/" target='appsmith'>appsmith</a>|All sql DBs|||| |
|<a href="https://appwrite.io/" target='appwrite'>appwrite.io</a>| DBs|Auth|Roles|Data|Tenancy |
|<a href="https:///" target=''></a>| DBs|Auth|Roles|Data|Tenancy |


