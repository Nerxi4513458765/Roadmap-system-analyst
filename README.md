# Роадмап системного аналитика : от нуля до портфолио и первых откликов

> Практико-ориентированная переработка роадмапа «С чего начать» из [Базы знаний по системному анализу](https://system-analyst.space/introduction/roadmap-start-here/).
> Основа и ссылки на теорию: system-analyst.space, лицензия CC BY-SA 4.0. Эта версия распространяется на тех же условиях.

---

## Как пользоваться

**Приоритеты тем**

- 🟢 **Обязательно** — без этого на первое собеседование идти рано
- 🟡 **Желательно** — повышает шансы, изучай после 🟢 того же этапа
- ⚪ **Потом** — справочник; читай, когда тема встретилась в вакансии или на проекте

**Правила**

1. **Пропорция 1 : 2.** На час чтения — минимум два часа практики. Если практика не сделана, этап не пройден.
2. **Каждый этап заканчивается артефактом** — файлом, который можно положить в портфолио.
3. **Не иди дальше, пока не пройден чекпоинт** этапа.
4. **Калибруй по рынку.** После этапа 1 у тебя будет таблица вакансий. Если в ней часто встречается технология из раздела ⚪, повышай её приоритет.

**Темп:** ориентиры ниже даны для 8–10 часов в неделю. Реальные сроки зависят от бэкграунда.

---

## Обзор маршрута

| # | Этап | Время | Артефакт |
|---|---|---|---|
| 1 | Роль и рынок | ~1 нед | Карта вакансий + описание роли |
| 2 | Требования | ~3 нед | Мини-пакет требований к одной фиче |
| 3 | Моделирование | ~2 нед | BPMN + sequence-диаграмма |
| 4 | Данные и SQL | ~4 нед | ERD + файл с 10 запросами |
| 5 | Как устроена система | ~1 нед | Схема «от клика до БД» |
| 6 | API | ~3 нед | OpenAPI-спецификация + описание метода |
| — | **Можно начинать откликаться** | | |
| 7 | Асинхронные интеграции (минимум) | ~2 нед | Описание топика + схема |
| 8 | Архитектура (минимум) | ~2 нед | ADR + C4 |
| 9 | Capstone-проект | ~4–6 нед | Полный аналитический пакет |
| 10 | Работа и собеседования | параллельно + 2–3 нед | Резюме, 3+ пробных интервью |

**Итого:** около 5–6 месяцев до сильного портфолио. Этапы 1–6 примерно за 3,5–4 месяца дают базу для первых откликов.

---

## Этап 1. Роль и рынок (~1 неделя)

**Цель:** понять, чем занимается СА, где он в команде, и что реально просят работодатели.

### Что изучить

| Тема | Приоритет | Комментарий |
|---|---|---|
| [Кто такой системный аналитик](https://system-analyst.space/introduction/who-is-system-analyst) | 🟢 | Роль, зона ответственности, результаты |
| [СА vs БА](https://system-analyst.space/introduction/ba_vs_sa) | 🟢 | Граница ролей |
| [Роли в команде и коммуникации](https://system-analyst.space/introduction/team-roles-and-communication) | 🟢 | С кем работаешь ежедневно |
| [SDLC](https://system-analyst.space/introduction/sdlc) | 🟢 | Где в цикле участвует аналитик |
| [Методологии (Agile, Scrum, Kanban)](https://system-analyst.space/introduction/methodologies) | 🟢 | Базовый уровень |
| [Артефакты требований и документации](https://system-analyst.space/introduction/requirements-and-documentation-artifacts) | 🟢 | Что аналитик производит |
| [Инструменты аналитика](https://system-analyst.space/introduction/tools-overview) | 🟡 | Jira, Confluence, Postman, диаграммные редакторы |
| [Кто такой бизнес-аналитик](https://system-analyst.space/introduction/who-is-business-analyst) | 🟡 | Для понимания соседней роли |
| [Англо-русский словарь](https://system-analyst.space/general/eng-ru-dictionary) | ⚪ | Справочник |

### Практика

- [ ] Собери **10–15 вакансий** системного аналитика (junior и стажировки в приоритете). Сделай таблицу: обязанности, технологии, домен, требуемый опыт.
- [ ] Посчитай, какие технологии встречаются чаще всего (SQL, REST, Kafka, BPMN, UML, Jira…). Это твоя **персональная калибровка** для всего роадмапа.
- [ ] Своими словами, в 5–7 предложениях, опиши разницу СА и БА.

**Артефакт:** таблица вакансий + одностраничное описание роли.

### Чекпоинт

Можешь ли ты объяснить:
- чем СА отличается от БА и от разработчика?
- на каких этапах SDLC работает аналитик и что он передаёт дальше?
- какие технологии из таблицы вакансий встречаются в большинстве объявлений?

---

## Этап 2. Требования (~3 недели)

**Цель:** научиться превращать размытый запрос бизнеса в понятные требования.

### Что изучить

| Тема | Приоритет | Комментарий |
|---|---|---|
| [Виды требований: бизнес](https://system-analyst.space/requirements/types-of-requirement/business-requirements), [пользовательские](https://system-analyst.space/requirements/types-of-requirement/user-requirements), [функциональные](https://system-analyst.space/requirements/types-of-requirement/functional) | 🟢 | Умей различать уровни |
| [Нефункциональные требования](https://system-analyst.space/requirements/types-of-requirement/non-functional) | 🟢 | Всегда с измеримыми значениями |
| [Бизнес-правила](https://system-analyst.space/requirements/types-of-requirement/business-rules) | 🟢 | Отличай от функциональных требований |
| [Сбор требований](https://system-analyst.space/requirements/collecting-requirements) | 🟢 | Интервью, уточняющие вопросы |
| [User Story](https://system-analyst.space/requirements/user-story/user-story) и [критерии приёмки](https://system-analyst.space/requirements/user-story/acceptance-criteria) | 🟢 | Формат + Given/When/Then |
| [Use Case](https://system-analyst.space/requirements/use-case) | 🟢 | Основной, альтернативные и исключительные сценарии |
| [Приоритизация](https://system-analyst.space/requirements/prioritization) | 🟡 | MoSCoW и аналоги |
| [INVEST](https://system-analyst.space/requirements/user-story/invest) | 🟡 | Проверка качества User Story |
| [BRD / FRD / SRS](https://system-analyst.space/requirements/brd-frd-srs) | 🟡 | Виды документов |

### Практика

- [ ] Выбери знакомый продукт или сервис (например, CRM, заказ доставки, запись на услугу) и опиши **одну фичу** по цепочке: бизнес-цель → пользовательская потребность → функциональные требования.
- [ ] Напиши **5 User Story** с критериями приёмки. Проверь каждую по INVEST.
- [ ] Опиши **один Use Case** с основным, альтернативным и ошибочным сценарием.
- [ ] Сформулируй **3–5 NFR** с цифрами (например, время отклика, доступность).
- [ ] На запрос «сделайте личный кабинет» подготовь **15 уточняющих вопросов** бизнесу.
- [ ] Расставь приоритеты 10 требований по MoSCoW и обоснуй выбор.

**Артефакт:** мини-пакет требований к одной фиче (2–3 страницы).

### Чекпоинт

- Можешь привести пример, где требование смешано с решением, и исправить его?
- Каждое NFR из твоего пакета измеримо?
- Можешь объяснить, когда нужна User Story, а когда Use Case?

---

## Этап 3. Моделирование (~2 недели)

**Цель:** показывать процессы и взаимодействия схемами, а не только текстом.

### Что изучить

| Тема | Приоритет | Комментарий |
|---|---|---|
| [BPMN](https://system-analyst.space/modeling/bpmn) | 🟢 | Роли, шлюзы, события, исключения |
| [UML](https://system-analyst.space/modeling/uml) | 🟢 | Минимум: sequence, activity, use case, class |
| [C4](https://system-analyst.space/modeling/c4) | 🟡 | Уровни Context и Container |
| [Event Storming](https://system-analyst.space/modeling/event-storming) | ⚪ | Когда работаешь с DDD-командами |
| [EPC](https://system-analyst.space/modeling/epc), [IDEF](https://system-analyst.space/modeling/idef) | ⚪ | Встречаются в legacy и госсекторе |

### Практика

- [ ] Нарисуй **BPMN As-Is и To-Be** для реального процесса (оформление заказа, обработка заявки) с ролями и исключениями. Инструменты: bpmn.io, diagrams.net.
- [ ] Нарисуй **sequence-диаграмму** для одного сценария между пользователем, фронтом, бэком и БД. Можно в PlantUML или Mermaid.
- [ ] Нарисуй C4 **Context** для простой системы.
- [ ] Найди чужую диаграмму в открытых источниках и найди в ней 3 недочёта.

**Артефакт:** BPMN-схема + sequence-диаграмма.

### Чекпоинт

- Читаешь чужую BPMN-схему без подсказок?
- Объясняешь, почему выбрал именно этот тип схемы?
- Нет «схем ради схем»: каждая отвечает на конкретный вопрос.

---

## Этап 4. Данные и SQL (~4 недели)

**Цель:** читать и проектировать структуры данных, писать запросы самостоятельно. SQL проверяют почти на любом собеседовании аналитика.

### Что изучить

| Тема | Приоритет | Комментарий |
|---|---|---|
| [Основы БД](https://system-analyst.space/data-and-sql/database-basics), [реляционные БД](https://system-analyst.space/data-and-sql/relational-databases/what-is-rdbms) | 🟢 | Таблицы, строки, связи |
| [Ключи](https://system-analyst.space/data-and-sql/relational-databases/database-schema-design/key) | 🟢 | PK, FK |
| [ER-диаграмма](https://system-analyst.space/data-and-sql/relational-databases/database-schema-design/entity-relationship-diagram) | 🟢 | Чтение и проектирование |
| [Нормализация](https://system-analyst.space/data-and-sql/relational-databases/database-schema-design/normalization) | 🟢 | До 3НФ |
| [Что такое SQL](https://system-analyst.space/data-and-sql/sql/what-is-sql), [JOIN](https://system-analyst.space/data-and-sql/sql/joins), [агрегация и группировка](https://system-analyst.space/data-and-sql/sql/aggregation-grouping) | 🟢 | Основа основ |
| [Подзапросы](https://system-analyst.space/data-and-sql/sql/subqueries), [оконные функции](https://system-analyst.space/data-and-sql/sql/window-functions) | 🟢 | Частые задачи на собеседованиях |
| [DML](https://system-analyst.space/data-and-sql/sql/sql-command-groups/dml), [DDL](https://system-analyst.space/data-and-sql/sql/sql-command-groups/ddl) | 🟡 | INSERT/UPDATE/DELETE, CREATE/ALTER |
| [Транзакции](https://system-analyst.space/data-and-sql/relational-databases/transactions/what-is-transaction), [ACID](https://system-analyst.space/data-and-sql/relational-databases/transactions/acid), [COMMIT/ROLLBACK](https://system-analyst.space/data-and-sql/relational-databases/transactions/commit-rollback) | 🟡 | Только идея и смысл |
| [Индексы: принцип работы](https://system-analyst.space/data-and-sql/relational-databases/indexes/how-indexes-work) | 🟡 | Зачем нужны и чем платим |
| [Денормализация](https://system-analyst.space/data-and-sql/relational-databases/database-schema-design/denormalization) | 🟡 | Когда дублирование осознанно |
| [Реляционные vs нереляционные](https://system-analyst.space/data-and-sql/relational-vs-norelational), [OLTP vs OLAP](https://system-analyst.space/data-and-sql/database-classes/oltp-vs-olap) | 🟡 | Уровень «когда что выбрать» |
| [SQL Best Practices](https://system-analyst.space/data-and-sql/sql/sql-best-practices), [EXPLAIN](https://system-analyst.space/data-and-sql/sql/explain) | 🟡 | После уверенного SELECT |
| [DCL](https://system-analyst.space/data-and-sql/sql/sql-command-groups/dcl), [TCL](https://system-analyst.space/data-and-sql/sql/sql-command-groups/tcl) | ⚪ | Справочник |
| [Уровни изоляции](https://system-analyst.space/data-and-sql/relational-databases/transactions/isolation-levels), [аномалии](https://system-analyst.space/data-and-sql/relational-databases/transactions/transaction-anomalies), [механизмы изоляции](https://system-analyst.space/data-and-sql/relational-databases/transactions/isolation-mechanisms), [WAL](https://system-analyst.space/data-and-sql/relational-databases/transactions/wal) | ⚪ | Внутренности СУБД |
| [Типы индексов](https://system-analyst.space/data-and-sql/relational-databases/indexes/index-types), [алгоритмы индексирования](https://system-analyst.space/data-and-sql/relational-databases/indexes/indexing-algorithms) | ⚪ | Углубление |
| [NoSQL: обзор](https://system-analyst.space/data-and-sql/norelational-databases/what-is-nosql) и [типы](https://system-analyst.space/data-and-sql/norelational-databases/type-nosql/) | ⚪ | Достаточно знать названия и сценарии |
| [BASE](https://system-analyst.space/data-and-sql/norelational-databases/base), [HTAP](https://system-analyst.space/data-and-sql/database-classes/hybrid-transactional-analytical-processing), [Persistent vs In-Memory](https://system-analyst.space/data-and-sql/database-classes/persistent-vs-in-memory) | ⚪ | Справочник |

### Практика

- [ ] Подними локально PostgreSQL или SQLite, загрузи любой открытый датасет и **ответь на 10 бизнес-вопросов** запросами.
- [ ] Реши **50+ задач** на платформах для практики SQL (например SQLBolt, pgexercises.com, SQL Academy, Stepik-курсы). Обязательно задачи на JOIN, GROUP BY/HAVING, подзапросы и оконные функции.
- [ ] Спроектируй БД для выбранного домена (например, CRM: клиенты, сделки, задачи, менеджеры): **ERD с PK/FK в 3НФ**.
- [ ] Для одного запроса посмотри `EXPLAIN` и объясни, что он показывает.

**Артефакт:** ERD + файл с 10 запросами и комментариями.

### Чекпоинт

- Пишешь JOIN + GROUP BY + оконную функцию **без подсказок**?
- Объясняешь, чем PK отличается от FK и зачем нормализация?
- Можешь коротко объяснить, когда SQL, а когда NoSQL?

---

## Этап 5. Как устроена система (~1 неделя)

**Цель:** перестать воспринимать приложение как чёрный ящик.

### Что изучить

| Тема | Приоритет | Комментарий |
|---|---|---|
| [Frontend](https://system-analyst.space/introduction/frontend), [Backend](https://system-analyst.space/introduction/backend) | 🟢 | Кто за что отвечает |
| Клиент-сервер и HTTP: запрос, ответ, заголовки, статусы | 🟢 | Смотри в DevTools своего браузера |
| [Полезные сервисы](https://system-analyst.space/general/useful-services) | 🟡 | Инструменты для работы с API и схемами |
| [Micro Frontend](https://system-analyst.space/introduction/mf) | ⚪ | Когда встретится в проекте |
| [Модель OSI](https://system-analyst.space/general/model-osi) | ⚪ | Достаточно общего понимания |

### Практика

- [ ] Открой DevTools → Network на любом сайте и разбери 3 запроса: метод, URL, статус, тело ответа.
- [ ] Нарисуй схему «что происходит от нажатия кнопки до записи в БД».

**Артефакт:** схема «от клика до БД».

### Чекпоинт

Можешь рассказать за 2 минуты путь запроса от браузера до базы и обратно?

---

## Этап 6. API (~3 недели)

**Цель:** читать и описывать API-контракты. Самый востребованный технический навык СА.

### Что изучить

| Тема | Приоритет | Комментарий |
|---|---|---|
| [Что такое API](https://system-analyst.space/api-and-integrations/what-is-api) | 🟢 | |
| REST: [принципы](https://system-analyst.space/api-and-integrations/api-styles-protocols/rest/rest-principles), [ресурсы](https://system-analyst.space/api-and-integrations/api-styles-protocols/rest/resources), [HTTP-методы](https://system-analyst.space/api-and-integrations/api-styles-protocols/rest/http-methods), [статусы](https://system-analyst.space/api-and-integrations/api-styles-protocols/rest/http-status-codes) | 🟢 | |
| [JSON](https://system-analyst.space/api-and-integrations/data-formats/json) | 🟢 | |
| [OpenAPI / Swagger](https://system-analyst.space/api-and-integrations/api-documentation/openapi) | 🟢 | Читать и писать |
| [Postman](https://system-analyst.space/api-and-integrations/api-documentation/postman) | 🟢 | Проверять API руками |
| [Идемпотентность](https://system-analyst.space/api-and-integrations/api-styles-protocols/rest/idempotency) | 🟢 | Ключевая тема для собеседований |
| [Аутентификация](https://system-analyst.space/api-and-integrations/api-security/authentication) и [авторизация](https://system-analyst.space/api-and-integrations/api-security/authorization) | 🟢 | Разница |
| [Пагинация](https://system-analyst.space/api-and-integrations/api-styles-protocols/rest/pagination), [фильтрация и сортировка](https://system-analyst.space/api-and-integrations/api-styles-protocols/rest/filtering-sorting) | 🟡 | |
| [Версионирование](https://system-analyst.space/api-and-integrations/api-styles-protocols/rest/api-versioning), [совместимость](https://system-analyst.space/api-and-integrations/api-design/backward-forward-compatibility) | 🟡 | |
| [JWT](https://system-analyst.space/api-and-integrations/api-security/jwt), [OAuth 2.0](https://system-analyst.space/api-and-integrations/api-security/oauth) | 🟡 | На уровне «как работает» |
| [Валидация входных данных](https://system-analyst.space/api-and-integrations/api-security/input-validation), [Rate Limiting](https://system-analyst.space/api-and-integrations/api-security/rate-limiting) | 🟡 | |
| [Webhooks vs Polling](https://system-analyst.space/api-and-integrations/api-styles-protocols/webhooks/webhooks-vs-polling), [WebSocket](https://system-analyst.space/api-and-integrations/api-styles-protocols/websokets/what-are-websockets) | 🟡 | Идея и сценарии |
| [Contract-first vs Code-first](https://system-analyst.space/api-and-integrations/api-design/contract-first-vs-code-first), [корреляция запросов](https://system-analyst.space/api-and-integrations/api-design/query-correlation) | 🟡 | |
| [API Gateway](https://system-analyst.space/api-and-integrations/integration-patterns/api-gateway) | 🟡 | |
| [XML](https://system-analyst.space/api-and-integrations/data-formats/xml), [SOAP](https://system-analyst.space/api-and-integrations/api-styles-protocols/soap/what-is-soap) | ⚪ | Повысь приоритет, если SOAP часто в вакансиях (банки, госсектор) |
| [gRPC](https://system-analyst.space/api-and-integrations/api-styles-protocols/grpc/grpc-concepts), [Protobuf](https://system-analyst.space/api-and-integrations/data-formats/protobuf) | ⚪ | Повысь приоритет по вакансиям |
| [GraphQL](https://system-analyst.space/api-and-integrations/api-styles-protocols/graphql/graphql-concepts), [YAML](https://system-analyst.space/api-and-integrations/data-formats/yaml) | ⚪ | Справочник |
| [HTTPS/TLS](https://system-analyst.space/api-and-integrations/api-security/https-tls), [CORS](https://system-analyst.space/api-and-integrations/api-security/cross-origin-resource-sharing), [mTLS](https://system-analyst.space/api-and-integrations/api-security/mtls), [Keycloak](https://system-analyst.space/api-and-integrations/api-security/keycloak) | ⚪ | Уровень «слышал и понимаю зачем» |
| [AsyncAPI](https://system-analyst.space/api-and-integrations/api-documentation/asyncapi), [gRPC Reflection](https://system-analyst.space/api-and-integrations/api-documentation/grpc-reflection) | ⚪ | |
| [BFF](https://system-analyst.space/api-and-integrations/integration-patterns/bff-pattern), [ESB](https://system-analyst.space/api-and-integrations/integration-patterns/esb), [Point-to-Point](https://system-analyst.space/api-and-integrations/integration-patterns/point-to-point), [оркестрация vs хореография](https://system-analyst.space/api-and-integrations/integration-patterns/orchestration-vs-choreography) | ⚪ | |
| [Тестирование API](https://system-analyst.space/api-and-integrations/api-testing/) | ⚪ | Зона QA, достаточно знать виды |

### Практика

- [ ] В Postman отправь запросы GET/POST/PUT/DELETE к открытому тестовому API (например, jsonplaceholder.typicode.com), сохрани **коллекцию**.
- [ ] Возьми готовую публичную OpenAPI-спецификацию и найди: эндпоинты, схемы, коды ошибок, требования к авторизации.
- [ ] Напиши **свою OpenAPI-спецификацию** на 3–4 метода (CRUD для сущности из твоей ERD) в Swagger Editor (editor.swagger.io).
- [ ] Опиши один метод по шаблону: [REST API](https://system-analyst.space/general/examples-of-doc/template-rest-api), ошибки, статусы, идемпотентность.

**Артефакт:** OpenAPI-файл + описание метода.

### Чекпоинт

- Читаешь чужую спецификацию и понимаешь, что и как вызывать?
- Объясняешь разницу PUT/PATCH, 401/403, и зачем нужен idempotency key?
- Можешь описать контракт метода так, чтобы разработчик не задал уточняющих вопросов по сути?

> **Точка старта откликов.** После этапа 6 у тебя есть требования, схемы, SQL и API-контракт. Для стажировок и junior-позиций этого часто достаточно. Начинай откликаться и параллельно иди дальше.

---

## Этап 7. Асинхронные интеграции: минимум (~2 недели)

**Цель:** понимать, чем асинхронное взаимодействие отличается от REST, и описывать простой контракт события.

### Что изучить

| Тема | Приоритет | Комментарий |
|---|---|---|
| [Что такое брокер сообщений](https://system-analyst.space/message-brokers-queues/what-is-message-broker) | 🟢 | |
| [Модели доставки](https://system-analyst.space/message-brokers-queues/delivery-models) (queue, pub/sub) | 🟢 | |
| [Гарантии доставки](https://system-analyst.space/message-brokers-queues/delivery-guarantees) | 🟢 | at-most / at-least / exactly-once |
| [Архитектура Kafka](https://system-analyst.space/message-brokers-queues/apache-kafka/kafka-architecture) | 🟢 | Topic, partition, producer, consumer group |
| [Partition Key Design](https://system-analyst.space/message-brokers-queues/apache-kafka/partition-key-design), [Ordering](https://system-analyst.space/message-brokers-queues/apache-kafka/ordering-guarantees) | 🟢 | Связь ключа и порядка |
| [Idempotent Consumer](https://system-analyst.space/message-brokers-queues/integration-patterns/idempotent-consumer) | 🟢 | |
| [Dead Letter Queue](https://system-analyst.space/message-brokers-queues/rabbitmq/dead-letter-queue), [Poison Message](https://system-analyst.space/message-brokers-queues/apache-kafka/poison-message) | 🟡 | Ошибки и retry |
| [Архитектура RabbitMQ](https://system-analyst.space/message-brokers-queues/rabbitmq/rabbitmq-architecture), [Kafka vs RabbitMQ](https://system-analyst.space/message-brokers-queues/kafka-vs-rabbitmq) | 🟡 | |
| [Outbox / Inbox](https://system-analyst.space/message-brokers-queues/integration-patterns/outbox-inbox-pattern) | 🟡 | Популярный вопрос на собеседованиях |
| [Шаблон Kafka-топика](https://system-analyst.space/general/examples-of-doc/template-kafka-topic) | 🟡 | |
| [Rebalancing](https://system-analyst.space/message-brokers-queues/apache-kafka/consumer-group-rebalancing), [Replication](https://system-analyst.space/message-brokers-queues/apache-kafka/replication), [Retention](https://system-analyst.space/message-brokers-queues/apache-kafka/data-retention), [Log Compaction](https://system-analyst.space/message-brokers-queues/apache-kafka/log-compaction), [Transactions](https://system-analyst.space/message-brokers-queues/apache-kafka/kafka-transactions), [Kafka как хранилище](https://system-analyst.space/message-brokers-queues/apache-kafka/kafka-as-storage) | ⚪ | Внутренности Kafka. Повысь приоритет, если Kafka в большинстве вакансий |
| [Message Router / Filter / Splitter](https://system-analyst.space/message-brokers-queues/integration-patterns/), [Competing Consumers](https://system-analyst.space/message-brokers-queues/integration-patterns/competing-consumers), [другие брокеры](https://system-analyst.space/message-brokers-queues/other-brokers) | ⚪ | Справочник |

### Практика

- [ ] Для сценария «оформление заказа» реши, **что синхронно (REST), а что асинхронно (событие)**, и нарисуй sequence-диаграмму.
- [ ] Опиши **контракт топика** по шаблону: ключ, схема сообщения, обработка ошибок, retry, DLQ.
- [ ] Объясни письменно в 5 предложениях, почему при at-least-once нужен идемпотентный consumer.

**Артефакт:** описание топика + схема.

### Чекпоинт

- Объясняешь, зачем брокер, и чем топик отличается от очереди?
- Понимаешь, как ключ влияет на порядок сообщений?
- Знаешь, что будет с сообщением, которое не удалось обработать?

---

## Этап 8. Архитектура: минимум (~2 недели)

**Цель:** говорить с архитектором и разработчиками на одном языке и фиксировать решения.

### Что изучить

| Тема | Приоритет | Комментарий |
|---|---|---|
| [Что такое архитектура ПО](https://system-analyst.space/architecture-and-design/what-is-software-architecture) | 🟢 | |
| [Монолит vs микросервисы](https://system-analyst.space/architecture-and-design/architectural-styles/microservices/monolith-vs-microservices), [проблемы микросервисов](https://system-analyst.space/architecture-and-design/architectural-styles/microservices/microservices-problems) | 🟢 | Компромиссы, а не «что лучше» |
| [Quality Attributes](https://system-analyst.space/architecture-and-design/quality-attributes) | 🟢 | Связь с NFR |
| [Основы масштабирования](https://system-analyst.space/architecture-and-design/scaling/scaling-basics), [кеширование](https://system-analyst.space/architecture-and-design/basic-components/cashe), [балансировка](https://system-analyst.space/architecture-and-design/scaling/load-balancing) | 🟢 | |
| [ADR](https://system-analyst.space/architecture-and-design/adr) и [шаблон ADR](https://system-analyst.space/general/examples-of-doc/template-adr) | 🟡 | Фиксация решений |
| [Event-Driven Architecture](https://system-analyst.space/architecture-and-design/architectural-styles/event-driven-architecture/what-is-eda) | 🟡 | |
| [CAP-теорема](https://system-analyst.space/architecture-and-design/scaling/cap-theorem), [репликация](https://system-analyst.space/architecture-and-design/scaling/replication) | 🟡 | Уровень идеи |
| [Observability](https://system-analyst.space/architecture-and-design/observability), [SLO/SLA/SLI](https://system-analyst.space/architecture-and-design/slo-sla-sli) | 🟡 | Для требований к логированию и надёжности |
| [Retry](https://system-analyst.space/architecture-and-design/architectural-patterns/retry-pattern), [Circuit Breaker](https://system-analyst.space/architecture-and-design/architectural-patterns/circuit-breaker) | 🟡 | Часто всплывают в NFR |
| [Bounded Context](https://system-analyst.space/architecture-and-design/bounded-context), [Clean Architecture](https://system-analyst.space/architecture-and-design/clean-architecture) | ⚪ | |
| [Saga](https://system-analyst.space/architecture-and-design/architectural-patterns/saga-pattern), [CQRS](https://system-analyst.space/architecture-and-design/architectural-patterns/command-query-responsibility-segregation), [Event Sourcing](https://system-analyst.space/architecture-and-design/architectural-patterns/event-sourcing), [Strangler Fig](https://system-analyst.space/architecture-and-design/architectural-patterns/strangler-fig-pattern), [Bulkhead](https://system-analyst.space/architecture-and-design/architectural-patterns/bulkhead-pattern), [Sidecar](https://system-analyst.space/architecture-and-design/architectural-patterns/sidecar-pattern), [Database per Service](https://system-analyst.space/architecture-and-design/architectural-patterns/database-per-service), [API Composition](https://system-analyst.space/architecture-and-design/architectural-patterns/api-composition) | ⚪ | Паттерны микросервисной эпохи. Saga и Outbox спрашивают чаще остальных |
| [Шардинг](https://system-analyst.space/architecture-and-design/scaling/sharding), [PACELC](https://system-analyst.space/architecture-and-design/scaling/pacelc-theorem), [Data Mesh](https://system-analyst.space/architecture-and-design/data-management/data-mesh), [Data Lake vs Warehouse](https://system-analyst.space/architecture-and-design/data-management/data-lake-vs-warehouse), [CDC](https://system-analyst.space/architecture-and-design/data-management/cdc), [Polyglot Persistence](https://system-analyst.space/architecture-and-design/data-management/polyglot-persistence) | ⚪ | Углубление |
| [Serverless](https://system-analyst.space/architecture-and-design/architectural-styles/serverless/what-is-serverless), [Blue-Green / Canary](https://system-analyst.space/architecture-and-design/blue-green-canary-deployment) | ⚪ | |
| [Архитектурные компромиссы](https://system-analyst.space/architecture-and-design/architectural-tradeoffs/) | 🟡 | Прочитай хотя бы Consistency vs Availability и Technical Debt |
| [System Design для аналитика](https://system-analyst.space/architecture-and-design/system-design-for-sa) | 🟡 | Для собеседований среднего уровня |

### Практика

- [ ] Напиши **ADR** «монолит или микросервисы» для своего учебного сервиса: контекст, варианты, решение, последствия.
- [ ] Возьми 5 своих NFR и покажи, как каждое влияет на архитектурные решения.
- [ ] Нарисуй C4 **Container**-диаграмму для сервиса.

**Артефакт:** ADR + C4 Container.

### Чекпоинт

- Объясняешь, почему микросервисы не всегда лучше монолита?
- Можешь по NFR «доступность 99,9 %» назвать, что это означает для системы?
- Читаешь C4-схему и задаёшь по ней вопросы архитектору?

---

## Этап 9. Capstone-проект (~4–6 недель)

**Цель:** собрать всё в один цельный проект, который можно показать работодателю.

### Шаг 1. Разбери эталонный кейс

Пройди [кейс «Расторжение договора»](https://system-analyst.space/task-and-artefacts/termination-of-the-contract/case-description) целиком: BR → FR → NFR → UC → REST → gRPC → статусы → ошибки → модель данных → sequence → Jira-задача.
Для каждого артефакта ответь: **почему он написан именно так?** Что бы ты изменил?

### Шаг 2. Сделай свой проект

Выбери домен, который тебе интересен (например, CRM: клиенты, сделки, задачи; или заявка на возврат товара). Подготовь:

- [ ] Бизнес-цель и **BR**
- [ ] **FR** и **NFR** (по шаблонам [FR](https://system-analyst.space/general/examples-of-doc/template-fr), [NFR](https://system-analyst.space/general/examples-of-doc/template-nfr))
- [ ] **User Stories + AC** или **Use Case** ([шаблон UC](https://system-analyst.space/general/examples-of-doc/template-uc))
- [ ] **BPMN To-Be**
- [ ] **Sequence-диаграмма** основного сценария
- [ ] **Модель данных + ERD**
- [ ] **OpenAPI-спецификация** (2–4 метода)
- [ ] **Статусы** сущности и **ошибки**
- [ ] **Требования к логированию** ([шаблон](https://system-analyst.space/general/examples-of-doc/template-logging)) и [матрица прав](https://system-analyst.space/general/examples-of-doc/template-permission-matrix)
- [ ] Описание задачи для разработки в стиле **Jira**
- [ ] 🟡 Контракт Kafka-топика, если в сценарии есть асинхронная часть

### Шаг 3. Оформи и покажи

- [ ] Собери всё в одном месте: Notion, GitHub-репозиторий, PDF или общая папка с оглавлением.
- [ ] Добавь **краткое описание**: какую задачу решает проект, какие допущения приняты.
- [ ] Попроси ревью у практикующего аналитика или в профильном сообществе и **внеси правки**.

**Артефакт:** портфолио-проект.

### Чекпоинт

- Любой артефакт можно объяснить: «зачем он, кто его читает, что с ним делает дальше»?
- Артефакты согласованы между собой: статусы в схемах совпадают со статусами в API, поля в ERD совпадают с полями в контракте?

---

## Этап 10. Работа и собеседования (параллельно этапам 6–9, затем ~2–3 недели)

### Когда начинать

- **После этапа 6** можно откликаться на стажировки и junior-позиции, не дожидаясь завершения всего роадмапа.
- Параллельно можно искать небольшие аналитические задачи на фриланс-биржах: это даёт реальный опыт и материал для портфолио.

### Что изучить

| Тема | Приоритет | Комментарий |
|---|---|---|
| [Вопросы и ответы для собеседований](https://system-analyst.space/general/interview-questions-and-answers) | 🟢 | |
| [Прохождение скрининга](https://system-analyst.space/general/passing-the-screening) | 🟢 | |
| [Как справиться с любой задачей](https://system-analyst.space/general/how-to-handle-any-task) | 🟡 | Алгоритм разбора задач |
| [Логические задачи](https://system-analyst.space/general/logical-tasks) | 🟡 | Часто на собеседованиях в крупных компаниях |
| [Вопросы для скрининга/ТИ/команды](https://system-analyst.space/general/questions) | 🟡 | И какие вопросы задавать самому |
| [Глоссарий](https://system-analyst.space/glossary/glossary) | ⚪ | Справочник |

### Практика

- [ ] Резюме: ссылка на портфолио, 3–5 артефактов, технологии из твоей таблицы вакансий.
- [ ] Составь список из **30 вопросов** (SQL, REST, требования, диаграммы) и отвечай вслух без шпаргалки.
- [ ] Проведи **минимум 3 пробных интервью** с другом, знакомым аналитиком или в сообществе.
- [ ] Выполни **2–3 тестовых задания** (или придумай аналогичные) и разбери ошибки.
- [ ] После каждого собеседования записывай вопросы, на которые не смог ответить, и возвращайся к нужным темам.

### Чекпоинт

- Можешь за 2 минуты рассказать, чем занимался в проекте, и какие артефакты создал?
- Нет вопросов из частого списка, на которые ты не можешь ответить?

---

## Углубление (после первого оффера или по требованиям вакансий)

Заглядывай сюда, когда тема встретилась в вакансии, на тестовом или на реальном проекте.

| Направление | Темы | Когда нужно |
|---|---|---|
| Внутренности БД | Уровни изоляции, MVCC, WAL, алгоритмы индексов, NoSQL-типы | Работа с высоконагруженными системами, вопросы на middle |
| API-стили | gRPC, Protobuf, GraphQL, SOAP, AsyncAPI | Конкретный стек проекта |
| Безопасность | mTLS, CORS, Keycloak, OAuth-потоки | Интеграционные и банковские проекты |
| Kafka глубже | Rebalancing, retention, compaction, transactions | Если Kafka — основной интеграционный инструмент |
| Паттерны | Saga, CQRS, Event Sourcing, Strangler Fig, Bulkhead, Sidecar | Микросервисные проекты, middle+ |
| Данные в архитектуре | Sharding, PACELC, CDC, Data Mesh, Data Lake vs Warehouse | Аналитические платформы, DWH |
| Моделирование | Event Storming, EPC, IDEF | DDD-команды, legacy и госсектор |
| Эксплуатация | Blue-Green, Canary, serverless | Проекты с DevOps-культурой |

---

## Дополнительный блок: бизнес-сторона (по желанию, 1–2 недели)

В оригинальном роадмапе бизнес-анализ раскрыт слабо. Если вакансии просят «БА/СА» или ты хочешь расти в сторону продукта, добавь:

- **Анализ стейкхолдеров** (матрица влияния и интереса)
- **Бизнес-кейс и оценка эффекта** (зачем делать фичу, во что она обойдётся, как измерим успех)
- **Метрики и KPI** (как определить, что изменение сработало)
- **Интервью с пользователями и заказчиками** (структура, вопросы, фиксация результата)
- **Улучшение процессов** (поиск узких мест в As-Is)

**Практика:** для фичи из твоего capstone напиши бизнес-кейс на 1 страницу и определи 3 метрики успеха.
Для углубления можно использовать BABOK Guide и книгу К. Вигерса о разработке требований.

---

## Трекер прогресса

- [ ] Этап 1: карта вакансий готова
- [ ] Этап 2: мини-пакет требований
- [ ] Этап 3: BPMN + sequence
- [ ] Этап 4: ERD + 10 SQL-запросов, решено 50+ задач
- [ ] Этап 5: схема «от клика до БД»
- [ ] Этап 6: OpenAPI-спецификация
- [ ] **Отправлены первые отклики**
- [ ] Этап 7: описание топика
- [ ] Этап 8: ADR + C4
- [ ] Этап 9: capstone опубликован
- [ ] Этап 10: 3+ пробных интервью пройдено
- [ ] Раз в 4 недели: пересмотрена таблица вакансий и обновлены приоритеты

---

*Основано на материалах [базы знаний по системному анализу](https://system-analyst.space/) (CC BY-SA 4.0). Тайминги и пропорции в этой версии — ориентировочные рекомендации, а не результат исследования: подстраивай их под себя.*
