# Netology_K8S_3.1 Моисеенко А.Н.
## Домашнее задание к занятию «Установка Kubernetes»
## Задание 1. Установить кластер k8s с 1 master node
- Подготовка работы кластера из 5 нод: 1 мастер и 4 рабочие ноды.
- В качестве CRI — containerd.
- Запуск etcd производить на мастере.
- Способ установки выбрать самостоятельно.
### Установка master node и 4 workernode
<img width="1030" height="303" alt="image" src="https://github.com/user-attachments/assets/ea66ae03-04f1-41e5-8bb9-3026ce555720" />
<img width="916" height="353" alt="image" src="https://github.com/user-attachments/assets/8a17fd32-4ba6-46a2-bbab-39781db73ab0" />

<img width="477" height="127" alt="image" src="https://github.com/user-attachments/assets/24dd41f7-872b-474e-8346-4516a360d9c0" />  
  
etcd установлен на мастер ноду  
<img width="682" height="57" alt="image" src="https://github.com/user-attachments/assets/e2c27fbb-a1c0-477a-a16a-3b3a19b46abd" />

## Задание 2*. Установить HA кластер
Установить кластер в режиме HA.
Использовать нечётное количество Master-node.
Для cluster ip использовать keepalived или другой способ.

Переобразую 2 worker ноды в  control-plane.  
Удаляю worker ноды: k8s-2 и k8s-3  
На мастер ноде  
<img width="857" height="208" alt="image" src="https://github.com/user-attachments/assets/cea8dd09-48fc-4cdb-899f-3be66d93a4bf" />  
На worker ноде  
<img width="1330" height="335" alt="image" src="https://github.com/user-attachments/assets/74a5754e-9950-4a9d-9124-29eb5300edfe" />

Создание сертификата на масер ноде  
<img width="915" height="80" alt="image" src="https://github.com/user-attachments/assets/5b34e0a2-6987-4903-9efe-1cddbabc5559" />  
Запрос команды для добавления
<img width="1312" height="43" alt="image" src="https://github.com/user-attachments/assets/12079834-bc43-4483-bcdf-95e9a372a54b" />
Добавление новой control-plane ноды  
<img width="849" height="189" alt="image" src="https://github.com/user-attachments/assets/f33943dc-ca20-42ec-a11a-dce3ef29a296" />







