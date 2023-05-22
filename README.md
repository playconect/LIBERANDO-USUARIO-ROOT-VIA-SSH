#### LIBERANDO O USUÁRIO ROOT PARA ACESSO REMOTO VIA SSH
**Configurando uma máquina linux para liberar acesso remoto via ssh para o usuário root.**

**Instalar openssh-server**
```shell
apt-get install openssh-server
```
**Configurar senha para o root**
```shell
sudo passwd root
```
**Edite o seguinte arquivo: /etc/ssh/sshd_config**

**Modifique a linha:**
```shell
PermitRootLogin no 
```
**Para:**
```shell
PermitRootLogin yes
```
**Agora reinicie o serviço de ssh: /etc/init.d/ssh restart**

