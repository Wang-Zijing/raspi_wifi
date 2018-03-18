依次复制下面的各行命令，然后右键粘贴到树莓派的终端窗口，并执行命令：

1.git clone https://github.com/Wang-Zijing/raspi_wifi

2.cd raspi_wifi

3.sudo make install

4.sudo apt-get update

5.sudo apt-get install util-linux procps hostapd iproute2 iw haveged dnsmasq

6.sudo systemctl enable create_ap

7.确保周围没有树莓派会自动连接的wifi，重启树莓派，在电脑上查找树莓派wifi名称：MyAccessPoint

8.电脑连接树莓派的wifi（密码：12345678）

9.在电脑上用vnc或putty连接树莓派的ip地址:10.0.0.1。

（如果要让树莓派连接周围新的wifi网络：

  在树莓派的终端窗口运行命令：sudo nano /etc/wpa_supplicant/wpa_supplicant.conf
  
  在打开的文件中更改或添加wifi账号密码，保存并退出。
  
  重启树莓派，就可以让树莓派连入周围新的wifi。）
  
  # Thanks for Oblique's work
create wifi by Raspberry Pi
