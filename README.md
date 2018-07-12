# docker_auth
example usage of cesanta/docker_auth

This is a ready-to use docker-compose solution of cesanta's docker_auth.
I've made two ways of auth - by pwd (commented) and by mogodb. The main
way is in mongo, so it is ready to go via mongo integration.

# How to launch?

```
1st console: docker-compose up
2nd console: docker exec -ti registry_mongo_1 sh -c /conf/import.sh
```

All u need is to configure acl.json and users.json by your needs. By default users and acls are taken from cesanta examples.

# How to test?

```
docker login https://127.0.0.1:5000
user: admin
pw: badmin
--- or ---
user: test
pw: 123
```

# Documentation:

https://github.com/cesanta/docker_auth/blob/master/examples/reference.yml

https://github.com/cesanta/docker_auth/blob/master/docs/Backend_MongoDB.md
