## Tudo muito fácil. O que mais eu posso fazer ?

Agora que entendemos sobre as formas e os tipos de pesquisa de forma básica, vamos aprender mais alguns comandos e funcionalidades utilizando as APIs do Elasticsearch, antes de partirmos para o Logstash e o Kibana.

#### Shutdown

Depois de tanto tempo no ar, vamos dar um descanço pro cara né ? Para finalizar o seu Elasticsearch, você pode OU pará-lo via __service management__  utilizando, por exemplo, o comando "_sudo systemctl stop elasticsearch_" OU enviando executando um `kill` no PID do seu processo. Como fizemos a instalação diretamente do .zip, usaremos a segunda forma:

```
$ jps | grep Elasticsearch
22223
$ kill 22223
```

Ou se você for mais _oldschool_:

```
$ ps -ef | grep -i elasticsearch | grep -v grep | awk '{print $2}'
22223
$ kill 22223
```

Próximo: [Contagem de Documentos](/pages/counting.md)
