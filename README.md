# Serega2780_infra

Serega2780 Infra repository


Terraform-2

поднят стенд из двух ВМ, созданных из разных образов
протестировано наличие на них соответствующего ПО mongodb и ruby
код инфтраструктуры разбит по модулям
затем по веткам: stage и prod
создавались buckets

Terraform-1

установлен terraform
создан файл main.tf со всеми настройками
определены и настроены input и output переменные
с помощью terraform развернула ВМ из образа, на ней автоматически запещен сервис puma
через web протестирован функционал сервиса puma


Bastion

bastion_IP = 35.189.195.32
someinternalhost_IP = 10.132.0.3

cloud-testapp
testapp_IP = 35.233.40.230
testapp_port = 9292

установлен и настроен gcloud
с помощью gcloud создана ВМ
написаны скрипты для установки Ruby, Mongodb, а также скрипт деплоя приложения


cloud-testapp

testapp_IP = 35.233.40.230
testapp_port = 9292

установлен и настроен gcloud
с помощью gcloud создана ВМ
написаны скрипты для установки Ruby, Mongodb, а также скрипт деплоя приложения






