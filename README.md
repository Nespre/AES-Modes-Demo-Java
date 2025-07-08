# AES Playground - ECB, CBC, OFB & CFB em Python e Java

Este repositório contém implementações práticas do algoritmo AES (Advanced Encryption Standard) em vários modos de operação (ECB, CBC, OFB, CFB), usando as linguagens Python e Java. Os scripts cobrem desde abordagens manuais até o uso de bibliotecas como `PyCryptodome` e `javax.crypto`.

> **Nota:** Este projeto é apenas para fins educacionais.

<br>

## 📑 Índice
- [Scripts Disponíveis](#-scripts-disponíveis)
- [Como Funciona?](#️-como-funciona)
- [Como Usar?](#-como-usar)
- [Parâmetros](#️-parâmetros)
- [Contribuição](#-contribuição)
- [Licença](#-licença)
<br><br>

## Scripts Disponíveis

### `aes_ecb_python.py` (ECB)

- **Linguagem:** Python  
- **Modo:** ECB  
- **Descrição:** Recebe texto e chave como entrada, normaliza a chave com SHA-256 e realiza a encriptação/decriptação na mesma execução.  
- **Exemplo:**  
  Entrada: `"Criptografia AES"`  
  → Saída: Texto cifrado em base64 + texto restaurado.

### `AesEcbJava.java` (Main + AESCipher.java)

- **Linguagem:** Java  
- **Modo:** ECB  
- **Descrição:** Permite ao usuário escolher entre cifrar ou decifrar um texto em tempo real com uma chave fornecida. Loop interativo até o usuário encerrar.  
- **Exemplo:**  
  Escolha → `"Encrypt"` → Entrada: `"Texto"`  
  → Saída: Encrypted + opção de reiniciar.

### `AesModesJava.java` (CBC, OFB, CFB)

- **Linguagem:** Java  
- **Modos:** CBC, OFB, CFB  
- **Descrição:** Mostra o mesmo texto sendo cifrado e decifrado com uma chave pré-definida nos três modos, exibindo os resultados em Base64.  
- **Exemplo:**  
  Texto original: `"ESTAMOS NA AULA DE CRIPTOGRAFIA"`  
  → Criptograma (Base64)  
  → Texto restaurado
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
<br>

## Como Usar?

```bash
git clone https://github.com/SEU_USUARIO/aes-java-modes.git
cd aes-java-modes
javac Main.java
java Main
```
_Requer Java 8 ou superior instalado._
<br><br>

## Contribuição
Sinta-se à vontade para contribuir! Abra um pull request ou crie um issue para discutir melhorias.
<br><br>

## Licença
Este projeto está licenciado sob a MIT License. Veja LICENSE para mais detalhes.
