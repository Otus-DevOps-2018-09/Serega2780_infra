# Serega2780_infra

Serega2780 Infra repository


Ansible-1

Поскольку командой rm -rf ~/reddit удалили каталог reddit, при следующем запуске 
ansible-playbook clone.yml произошел повторный запуск task Clone repo,
чтобы заново создать этот каталог. Поэтому статус changed: [appserver]

Установлен Ansible. Поскольку на ВМ в GC по умолчанию установлен python 3, пришлось в inventory файл добавить строку инициализации
с правльным путем до python на удаленной ВМ. Этот вариант не описывался в методичке к ДЗ ansible_python_interpreter= \
/usr/bin/python3

Выполнены все примеры из ДЗ.

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
cloud-testapp
testapp_IP = 35.233.40.230
testapp_port = 9292

установлен и настроен gcloud
с помощью gcloud создана ВМ
написаны скрипты для установки Ruby, Mongodb, а также скрипт деплоя приложения



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


