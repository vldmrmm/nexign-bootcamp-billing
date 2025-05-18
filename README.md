# Baby Billing Service
## Постановка задачи на разработку биллинговой системы с 4 микросервисами:
  * [CDR](https://github.com/vldmrmm/nexign-bootcamp-billing/blob/main/Services/CDR.pdf) - Сервис эмулирует работу коммутатора: параллельно генерирует записи звонков в хронологическом порядке, которые затем собираются в CDR файл и отпралвяются в BRT;
  * [BRT](https://github.com/vldmrmm/nexign-bootcamp-billing/blob/main/Services/BRT.pdf) - Сервис хранит данные абонентов "Ромашки" в БД, он обрабатывает приходящие CDR-файлы, отбирает записи абонентов "Ромашки" и сохраняет их в БД. Звонок отправляется на тарификацию в HRS, после чего в BRT приходит сумма списания, сервис меняет баланс;
  * [HRS](https://github.com/vldmrmm/nexign-bootcamp-billing/blob/main/Services/HRS.pdf) - Сервис хранит данные о тарифах, а также хранит оставшиеся ресурсы абонента, производит расчет суммы списания, списывает ресурсы и отправляет сумму в BRT.
  * [CRM](https://github.com/vldmrmm/nexign-bootcamp-billing/blob/main/Services/CRM.pdf) - Сервис, предоставляющий абоненту и менеджеру различный набор прав.

## UML:

* ### [Use Case diagram](https://github.com/vldmrmm/nexign-bootcamp-billing/blob/main/UML/Use%20Case.png)

* ### [Activity diagram](https://github.com/vldmrmm/nexign-bootcamp-billing/blob/main/UML/activity.svg)


## [Swagger file](https://github.com/vldmrmm/nexign-bootcamp-billing/blob/main/vldmrmm-CRM-v1-resolved.yaml)

## [Открыть в Swagger Editor](https://editor.swagger.io/?url=https://raw.githubusercontent.com/vldmrmm/nexign-bootcamp-billing/blob/main/vldmrmm-CRM-v1-resolved.yaml)
