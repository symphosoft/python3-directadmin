# Python3  Directadmin

installation

python setup.py install

## Examples 

### List all users

from directadmin import api

a = api.Api("admin", "password", "hostname.com", 2222)
print a.list_all_users()


### Connect using HTTPS and list all users

from directadmin import api

a = directadmin.Api("admin", \
                      "password", \
                      "hostname.com", \
                      2222, \
                      True)
print a.list_all_users()
