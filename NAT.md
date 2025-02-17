# Роутеры

Настройку выполняем на ISP

`mkdir /etc/nftables`

`nano /etc/nftables/isp.nft`

указываем интерфейс, идущий в сторону Интернета

![{833E1262-2507-4C97-85EE-C0846F6C7362}](https://github.com/user-attachments/assets/fea07df7-475c-42e8-9580-5d7dd88d5d96)

`nano /etc/nftables.conf`

![{AE14C990-4CBC-4545-9471-DC700ED7C7A3}](https://github.com/user-attachments/assets/a8d3ffd9-b036-4320-a48c-25e566ef586c)

`systemctl enable nftables`

`systemctl start nftables`

`nano /etc/sysctl.conf`

раскомменчиваем строку

![{05EA3F8A-3D78-4875-9A17-F91B3556D3D0}](https://github.com/user-attachments/assets/5132185d-5ee8-472f-9675-bc2ffd3d0c2d)

`sysctl -p`

перезагружаем isp, если не работает


# Сервера
`mkdir /etc/nftables`

`nano /etc/nftables/hq-rtr.nft`

![{E5451729-AEC9-429D-B7AB-C00383EF8A27}](https://github.com/user-attachments/assets/9c2534d9-86a5-45d8-b7db-84328ae674eb)

`nano /etc/nftables.conf`

![{300D918B-7D2A-40CB-89D9-3B80BF1FA428}](https://github.com/user-attachments/assets/9e3301cb-a7eb-4b66-a2ad-6db21c707571)

`systemctl enable nftables`

`systemctl start nftables`

`nano /etc/sysctl.conf`

раскомменчиваем строку

![{D5AA0394-A03F-4276-916E-714C2FDA31B2}](https://github.com/user-attachments/assets/4bb925de-741c-4123-a929-25e2722995d5)

`sysctl -p`

перезагружаем роутер, если не работает



