### Админка Keycloak:
http://localhost:8080/admin

Логин/пароль: admin/admin

Внутри зайти в realm reports-realm

1. Добавить пользователя (users - add user)
2. Выставить email из airlow/db/breadcrumbsCrmClients.db таблицы crm_client
3. Пароль: credentials - set password, temporary = off

Добавить несколько пользователей из этой же таблицы, указав емайлы, иначе отчёт не откроется.

### Отчёты в DAG

http://localhost:8081/home
Логин/пароль: admin/admin

Включаем user_reports_etl

Жмём "Trigger DAG"

### Проверка UI

http://localhost:3000

Входим через Keycloak под одним из пользователей из airlow/db/breadcrumbsCrmClients.db таблицы crm_client
Жмём Download Report