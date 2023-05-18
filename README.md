# Step 1

tools needed:
* docker-desktop + kubernetes
* docker-compose
* vault-cli


### HARD WAY:
* create python app (flask+db)

### EASY START
1. find python app + db + tests if possible (was looking into: https://github.com/jennielees/flask-sqlalchemy-example  haven't tested it)
2. fork/repush it somewhere to your space

#### Jenkins

1. create deploy.sh script which will deploy jenkins helm chart to local kubernetes(docker-deploy)
should be preinstalled plugins
* casc plugin
* jobdsl plugin

2. create job configuration via jobdsl (casc) with `pipeline` type
* git -> should be pointed to your repo with APP
* creds - missed for now

3. change jenkins welcome message to "Hi, its version '$VAR_NAME'"

where $VAR_NAME - variable from deploy.sh script like

```
VAR_NAME = '123QWE'
```



# Step 2

TODO: in progress


