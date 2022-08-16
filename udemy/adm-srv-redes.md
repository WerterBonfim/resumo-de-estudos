# Administração de Servidores e Serviços de Rede

Meu resumo pessoal do curso:
<https://www.udemy.com/course/adm-srv-redes/>


Propósito do curso
- Descrever os conceitos de detalhes do funcionamento de cada protocolo
- Demostrar a implmentação dos protocolos em servidores Windows e Linux.


a historia da internet legandaddo


16 bits permitem 65536 combinações (0 a 65536)

* No cliente, uma porta aleatória acima de 1023 é designada para
estabelecer a conexão (open ativo) "ephemeral ports"

* Windows Vista> intervalo recomendado pelo IANA de 49152 a 65535
* GNU/Linux utilizam intervalo de 32768 a 60999

* No servidor, temos portas específicas abertas paara cada serviço (open passivo).


Socket: Junção de IP e porta: 192.168.1.20:80



~~~bash
nano /etc/services
~~~
 

~~~powershell
C:/Windows/System32/drivers/etc/services
~~~


Faixa de números de portas
* 0 a 1023      = Portas conhecidas (Contato)
* 1024 a 49151  = Portas registradas
* 49152 a 65535 = Portas privadas e/ou Dinâmicas

```bash

# -p = Exibe o PID que abriu a respectiva porta
# -t = Exibe portas TCP
# -u = Exibe portas UDP
# -a = Exibe todas as portas abertas
# -n = 

netstat -apt
netstat -napt
netstat -naptu
```

State
- LISTENING = open passivo, serviço de rede aberto aguardo alguem se conectar
- ESTABLISHED = conexão estabelecida

UDP não tem estado, apenas entrega. Se não chegou a aplicação que decide
