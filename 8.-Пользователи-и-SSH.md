# HQ_SRV и BR_SRV

Сделать на HQ_SRV и на BR_SRV.

Создаем пользователя sshuser.

`useradd sshuser -u 1010 -U` - создание пользователя

`passwd sshuser` - задать пароль пользователю

`вводим пароль пользователя` - P@ssw0rd

`повторяем ввод пароля` - P@ssw0rd

Далее, при необходимости, устанавливаем sudo.

`apt install sudo -y`

Заходим в `visudo` и прописываем нашего пользователя.

![image](https://github.com/user-attachments/assets/24bb4e8f-abcb-41b8-ba85-8c66d1a563d0)

# SSH

Создадим файл баннера, допустим `banner_ssh` и напишем текст ( можно написать без =, Authorized Access Only )

`nano /etc/banner_ssh`

![{BF335577-9E9F-4135-89C3-B0830770B5D6}](https://github.com/user-attachments/assets/8a426fbb-a96d-43a2-b65c-36b329bd54b5)

Пропишем выделенные параметры в конфигурационный файл

`nano /etc/ssh/sshd_config`

![{E91DC01B-8C2A-43E1-9D73-D3914B014F7D}](https://github.com/user-attachments/assets/adcf9638-da81-47b1-bbd9-025d0d94c759)

# Проверка SSH

Подключаемся с `HQ-RTR` указав имя созданного пользователя, ip-адрес `HQ-SRV` и порт 2024. Далее вводим пароль.

![{1A05CBA5-CEBE-43F4-A768-249D215EFAB9}](https://github.com/user-attachments/assets/04e359eb-0149-41b7-803b-2a238d7a1fe4)

После ввода пароля должно быть вот так:

![{C3BC6A4A-634B-437A-8847-F8EC982799DE}](https://github.com/user-attachments/assets/5dc9c13b-0a1b-4f48-9ed6-36961ac5b88a)

Далее прописываем `sudo su`, если пароль не запросился и вы вошли под `root`, то всё сделано правильно

![{C4B0A6FB-6E1D-450D-BAD0-238D014F3A21}](https://github.com/user-attachments/assets/72c90087-1907-406f-adbe-2e21b13b99a8)

# HQ-RTR и BR-RTR

Создадим пользователя `net_admin` и зададим ему пароль `P@ssw0rd`

![{4A665BD7-F8E4-4C7F-9474-E0FA346F40A5}](https://github.com/user-attachments/assets/fb918ff7-4d9c-41bb-b6fd-c47e0d91f386)

`visudo`

![{06741716-AFD5-4626-8F67-09AB943C5326}](https://github.com/user-attachments/assets/5f16df41-76a5-4412-9073-198056894a7e)

