# Gerenciador-de-Tabela-de-Simbolos

# Autores
- Isabella Monte Santa Cruz
- Ivanildo Marques de Souza Filho
- Ramon Freire Alencar

## Sobre o projeto
Este projeto implementa um Gerenciador de Tabela de Símbolos utilizando Pilhas e Hash Tables (dicionários em Python), simulando o comportamento de compiladores no gerenciamento de variáveis e escopos aninhados.

## Tecnologias Utilizadas
- Python
- Dicionários (Hash Tables)
- Listas (Pilhas)
- Google Colab

## Requisitos
- Python 3.8 ou superior

Verifique a instalação do Python com:

```
python --version
```
ou

```
python3 --version
```
## Como Executar

### 1. Baixe ou clone o projeto

Clone o repositório utilizando a URL do repositório:
```
https://github.com/Zabella0751/Gerenciador-de-Tabela-de-Simbolos.git
```
Ou baixe os arquivos do projeto.

### 2. Acesse a pasta do projeto
```
cd projeto
```

### 3. Execute o programa

- No Windows:
```
python tabela_simbolos.py
```
- No Linux ou macOS:
```
python3 tabela_simbolos.py
```

## Funcionalidades

### 1. declarar(variavel, tipo)
Declara uma variável no escopo atual.

Exemplo:
```
tabela.declarar("idade", "int")
```

### 2. buscar(variavel)
Procura uma variável do escopo mais interno para o mais externo.

Exemplo:

```
tabela.buscar("idade")
```

### 3. entrar_escopo()
Cria um novo escopo e o adiciona à pilha.

Exemplo:
```
tabela.entrar_escopo()
```

### 4. sair_escopo()
Remove o escopo atual da pilha.

## Exemplo de Uso
Ao executar o programa, serão realizadas algumas operações de demonstração:
```
tabela.declarar("x", "int")
tabela.declarar("nome", "string")

tabela.entrar_escopo()

tabela.declarar("y", "float")

tabela.buscar("x")
tabela.buscar("y")

tabela.sair_escopo()
```
Saída esperada:

Variável 'x' declarada como 'int'.
Variável 'nome' declarada como 'string'.

>Novo escopo criado.

Variável 'y' declarada como 'float'.

'x' encontrada com tipo 'int'.
'y' encontrada com tipo 'float'.

>Escopo removido.

Exemplo:
```
tabela.sair_escopo()
```

