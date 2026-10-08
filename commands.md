netsh interface ip set address "Ethernet" static 192.168.100.20 255.255.255.0
echo 192.168.100.10 opsi.lab.local opsi >> C:\Windows\System32\drivers\etc\hosts
netsh advfirewall firewall add rule name=ping protocol=icmpv4:8,any dir=in action=allow
ping opsi.lab.local
