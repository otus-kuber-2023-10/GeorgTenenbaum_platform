# GeorgTenenbaum_platform
GeorgTenenbaum Platform repository

В рамках ДЗ №8 сделано:

Развернул кластер из ДЗ №7.
Создал необходимые по заданию CR, CRD, deploy-operator, service-account, role, role-binding, bacis_crd. 
Создал docker-образ локально.
Создал необходимые templates по заданию.
Удалил Useless CR. 
Добавил описание обязательных полей в CRD через "required" (image,database, password, storage_size). 
Заполнил БД данными и проверил:

kubectl exec -it $MYSQLPOD -- mysql -potuspassword -e "select * from test;" otus-database
mysql: [Warning] Using a password on the command line interface can be insecure.
+----+-------------+
| id | name |
+----+-------------+
| 1 | some data |
| 2 | some data-2 |
+----+-------------+