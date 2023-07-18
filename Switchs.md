<h1 align="center"> Comandos básicos de Switch </h1>

<h3 align="center"> Referência Cisco IOS </h3>

![Badge em Desenvolvimento](http://img.shields.io/static/v1?label=STATUS&message=EM%20DESENVOLVIMENTO&color=GREEN&style=for-the-badge)

<h2 > Acesso aos switchs </h2>

```
telnet [Ip]
```
Acessa via Telnet o switch


<h2 > Help de comandos </h2>

```
?
```
Lista o Help do comando selecionado

<h2 >Modo Privilegiado </h2>

```
enable
```
Acessa o modo privilegiado, autorizando um número maior de comandos no switch

<h2 >Modo de Configuração </h2>

```
configure terminal
```
Acessa o modo de configuração, autorizando todos os comandos no switch

```
int f1/0
```
Acessa a porta no modo configuração

```
sw mode trunk
```
ativa o modo trunk

```
sw trunk allowed vlan [1,2,3]
```
seta as vlans permitidas no trunk

```
sw mode acces
```
ativa o modo access

```
sw acces vlan [vlan id]
```
seta a vlan referente a porta

```
exit
```
Sai do modo de configuração.

<h2 >Visualizar status das interfaces </h2>

```
sh vtp status
```
Exibe o status do Vlan Trunk Protocol

```
vtp mode transparent
```
altera o modo vtp para transparente dentro do Configure Terminal

```
sh int status
```
Exibe todas as portas e o status atual

<h2 >Exibir configurações </h2>

```
sh run
```
Exibe todas as configurações

```
sh run vlan [vlan name]
```
Exibe a configuração da vlan

```
sh run int f1/0
```
Exibe a configuração da interface

```
sh int f1/0
```
Exibe status da interface

<h2 >Exibir os vizinhos do switch </h2>

```
sh cdp nei
```
Exibe todos os switchs vizinhos
