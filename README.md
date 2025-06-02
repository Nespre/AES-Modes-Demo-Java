# Encriptação AES em Java – Modos CBC, OFB e CFB

Este projeto em Java demonstra a encriptação e desencriptação de um texto utilizando o algoritmo **AES** com três modos de operação diferentes: **CBC**, **OFB** e **CFB**. 
A chave fornecida é transformada com SHA-256 para obter o comprimento adequado, e um vetor de inicialização (IV) fixo de 16 bytes é usado (apenas para fins didáticos).
<br><br>

## Índice
- [Funcionalidades](#funcionalidades)
- [Como Funciona?](#como-funciona)
- [Exemplo de Resultado](#exemplo-de-resultado)
- [Como Usar?](#como-usar)
- [Contribuição](#contribuição)
- [Licença](#licença)
<br><br>

## Funcionalidades
- Conversão da chave de entrada para chave AES válida usando SHA-256
- Encriptação e desencriptação de uma mensagem de texto
- Suporte aos modos AES: CBC, OFB e CFB
- Codificação e decodificação do resultado em Base64
<br><br>

## Como Funciona?
1. O utilizador define um texto a encriptar e uma chave de 32 caracteres.
2. A chave é convertida em bytes e normalizada com o algoritmo SHA-256 para gerar uma chave AES válida.
3. Usa um IV fixo de 16 bytes a zeros (para fins didáticos).
4. Aplica encriptação com AES nos modos CBC, OFB e CFB.
5. Mostra o criptograma em Base64 e o texto desencriptado.

Cada modo é executado individualmente e imprime os resultados no terminal.
<br><br>

## Exemplo de saída
```
===Modo CBC===
Criptograma 		Wh485OT2H9fYjdRgeUEf8gi6WN4D3PChTLZBIk9eLsg=
Texto Decifrado 	ESTAMOS NA AULA DE CRIPTOGRAFIA
===Modo OFB===
...
```
<br><br>

## Como Usar?

1. Clone o repositório:
`git clone https://github.com/SEU_USUARIO/aes-java-modes.git`
2. Navegue até o diretório:
`cd aes-java-modes`
3. Compile e execute o programa:
`javac Main.java`
`java Main`

_Requer Java 8 ou superior instalado._
<br><br>

## Como Usar?

```bash
git clone https://github.com/SEU_USUARIO/aes-java-modes.git
cd aes-java-modes
javac Main.java
java Main
```
<br><br>

## Contribuição
Sinta-se à vontade para contribuir! Abra um pull request ou crie um issue para discutir melhorias.
<br><br>

## Licença
Este projeto está licenciado sob a MIT License. Veja LICENSE para mais detalhes.
