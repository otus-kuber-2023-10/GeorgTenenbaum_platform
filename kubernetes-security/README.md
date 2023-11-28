# GeorgTenenbaum_platform
GeorgTenenbaum Platform repository

В рамках ДЗ №6 сделано:

task01:

Создал service-account bob и предоставил ему роль admin в рамках всего кластера.
Создал service-account dave без доступа к кластеру.

task02:

Создал namespace prometheus.
Создал service-account carol в этом Namespace.
Дал доступ всем service-account в namespace prometheus возможность делать команды get, list, watch в отношении Pods всего кластера.

task03:

Создал namespace dev.
Создал service-account jane в namespace dev.
Дал jane роль admin в рамках namespace dev.
Создал service-account ken в namespace dev.
Дал ken роль view в рамках namespace dev.