# mkdir /etc/nftables

# nano /etc/nftables/isp.nft
указываем интерфейс, идущий в сторону Интернета

![{833E1262-2507-4C97-85EE-C0846F6C7362}](https://github.com/user-attachments/assets/fea07df7-475c-42e8-9580-5d7dd88d5d96)

# nano /etc/nftables.conf

![{AE14C990-4CBC-4545-9471-DC700ED7C7A3}](https://github.com/user-attachments/assets/a8d3ffd9-b036-4320-a48c-25e566ef586c)

# nano /etc/sysctl.conf

раскомменчиваем строку

![{05EA3F8A-3D78-4875-9A17-F91B3556D3D0}](https://github.com/user-attachments/assets/5132185d-5ee8-472f-9675-bc2ffd3d0c2d)

# sysctl -p

перезагружаем isp, если не работает


