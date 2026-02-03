export MYSQL_ROOT_PASSWORD="strong-password"
helm install --set mysqlRootPassword=$MYSQL_ROOT_PASSWORD -n airbyte-v2 my-mysql bitnami/mysql
