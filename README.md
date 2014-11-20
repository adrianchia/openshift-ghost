Openshift-Ghost
===============
This project runs [Ghost](https://github.com/TryGhost/Ghost), a free, open, simple blogging platform created and maintained by [John O'Nolan](http://twitter.com/JohnONolan) + [Hannah Wolfe](http://twitter.com/ErisDS) + an amazing group of [contributors](https://github.com/TryGhost/Ghost/contributors).

For more information about Ghost, visit [http://ghost.org](http://ghost.org) • docs on [http://support.ghost.org/](http://support.ghost.org/)

Running Ghost on OpenShift
--------------------------
### MySQL version (default)
- Execute the following command via rhc, or create from OpenShift web console.

        rhc app create ghost nodejs-0.10 --env NODE_ENV=productionmysql --from-code https://github.com/adrianchia/openshift-ghost.git

### Sqlite3
To adjust to Sqlite3 version, fork this repository, change pre_start_nodejs and pre_restart_nodejs and set  NODE\_ENV=production,

execute command in MySQL version with different NODE_ENV and point the code to your forked repository.