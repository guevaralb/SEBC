# The database type
# Currently 'mysql', 'postgresql' and 'oracle' are valid databases.
com.cloudera.cmf.db.type=mysql

# The database host
# If a non standard port is needed, use 'hostname:port'
com.cloudera.cmf.db.host=ip-54-157-31-236:3306

# The database name
com.cloudera.cmf.db.name=scm

# The database user
com.cloudera.cmf.db.user=root

# The database user's password
com.cloudera.cmf.db.password=1234

# The db setup type
# By default, it is set to INIT
# If scm-server uses Embedded DB then it is set to EMBEDDED
# If scm-server uses External DB then it is set to EXTERNAL
com.cloudera.cmf.db.setupType=EXTERNAL
