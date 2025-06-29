# inventory-service

## 参考
https://www.youtube.com/watch?v=sNu_9aqSk5Y&list=PLSVW22jAG8pDeU80nDzbUgr8qqzEMppi8&index=5&ab_channel=ProgrammingTechie

## はまったポイント
* Docker compose.ymlの記載が間違っており、order-serviceとDBボリュームが重複していることでエラーが発生した。正規の記載に直すことで解消
* Flywayがアプリケーション起動時にエラーになる
mvn flyway:repair -Dflyway.url=jdbc:mysql://localhost:3306/inventory_service -Dflyway.user=root -Dflyway.password=mysql
