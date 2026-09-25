# calculadora

# Projeto RPC em Python

Projeto desenvolvido em Python utilizando o protocolo **XML-RPC** para realizar comunicação entre um cliente e um servidor.

## Sobre o projeto

O servidor disponibiliza três funções remotamente:

* Soma
* Subtração
* Multiplicação

O cliente se conecta ao servidor através da porta **8000** e executa as funções remotamente.

## Tecnologias utilizadas

* Python 3
* XML-RPC
* `xmlrpc.server`
* `xmlrpc.client`

## Como executar

Primeiro, abra um terminal e execute o servidor:

```bash
python servidor.py
```

Depois, abra outro terminal e execute o cliente:

```bash
python cliente.py
```

## Resultado esperado

```text
10 + 5 = 15
10 - 5 = 5
10 x 5 = 50
```

## Funcionamento

O arquivo `servidor.py` cria um servidor XML-RPC na porta 8000 e registra as funções que poderão ser chamadas pelo cliente.

O arquivo `cliente.py` utiliza `xmlrpc.client.ServerProxy` para se conectar ao servidor e realizar as operações remotamente.
