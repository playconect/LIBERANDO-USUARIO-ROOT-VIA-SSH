### LIBERANDO O USUÁRIO ROOT PARA ACESSO REMOTO VIA SSH

Configurando uma máquina linux para liberar acesso remoto via ssh para o usuário root no Conectiva Linux 10. 

Edite o seguinte arquivo: **/etc/ssh/sshd_config**   

Modifique a linha:   
```shell
PermitRootLogin no 
```   
Para:   
```shell 
PermitRootLogin yes
```   

**Agora reinicie o serviço de ssh:***
```shell
service sshd stop
service sshd start 
```   

