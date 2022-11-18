# Tracer de Pacotes - Configurar Interfaces de Roteador

Atribuição de IPv4 e IPv6 a rotedores e PCs em uma topologia de Rede simples elaborada com a utilização do Packet Tracer

### 📋 Pré-requisitos

É necessário ter o Packet Tracer instalado no computador bem como o Java para rodar o programa

### 🔧 Configuração das interfaces GigabitEthernet e Serial R1

Configuração de R1 e LAN.
Configuração ipv4 para PC1, PC2 e Gateway padrão na GUI do Packet Tracer.
Portas GigabitEthernet  /25 e Serial  /30.

```
config t
	interface g0/0
	ip address 172.16.20.1 255.255.255.128
	no shutdown
	interface g0/1
	ip address 172.16.20.129 255.255.255.128
	no shutdown
	interface s0/0/0
	ip address 209.165.200.225 255.255.255.252
	no shutdown
	end	
copy running-config startup-config



```

## 🔧 Configuração das interfaces GigabitEthernet e Serial R2

Configuração ipv6 R2 e LAN + Link local
Configuração de ipv6 PC3, PC4 Gateway padrão ipv6


```
config t
	interface g0/0
	ipv6 address 2001:db8:c0de:12::1/64
	no shutdown
	interface g0/1
	ipv6 address 2001:db8:c0de:13::1/64
	no shutdown	
	interface s0/0/1
	ipv6 address 2001:db8:c0de:11::1/64
	no shutdown
	ipv6 address fe80::2 link-local
	end
copy running-config startup-config

```


## 🛠️ Construído com

* [Packet Tracer](https://www.packettracernetwork.com/download/download-packet-tracer.html) - Sofware para criação de topologia de rede
 
## 📌 Versão


Usado [Cisco Packet Tracer 8.2](https://www.packettracernetwork.com/download/download-packet-tracer.html) Para a utulização do Cisco Packet Tracer é necessário ter um conta no netacad
Site [Cisco Networking Academy](https://www.netacad.com/)


## ✒️ Autores


* **Um desenvolvedor** - Rodrigo-oss-prog.

 😊
