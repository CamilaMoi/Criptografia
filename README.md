# Criptografia — Cifra de Vigenère

> Repositório educativo para treinar conceitos de **criptografia clássica** usando a **cifra de Vigenère** em Python.

## Sobre

Este projeto reúne uma implementação simples da Vigenère e materiais de estudo. A ideia é praticar **criptografia  clássica**, manipulação de strings, testes e boas práticas de linha de comando — tudo com foco **didático**.

**O que você encontra aqui**

* Funções para **criptografar** usando uma *key* (palavra‑chave).

* Normalização de alfabeto (maiúsculas/minúsculas), remoção opcional de não‑letras.

* Exercícios e anotações para estudo.

> Observação: a Vigenère é uma cifra **histórica**. Não use em produção para proteger dados reais.

---

## Requisitos

* **Python** 3.10 ou superior
* (Opcional) `pipx` ou `virtualenv` para isolar dependências

---

## &#x20;Início rápido

1. **Clone** o repositório

   ```bash
   git clone https://github.com/CamilaMoi/Criptografia.git
   cd Criptografia
   ```

2. (Opcional) **Crie um ambiente virtual**

   ```bash
   python3 -m venv .venv && source .venv/bin/activate
   ```

---

## &#x20;Uso (Terminal)

### Criptografar

* Dê as informações pedidas pelo programa

### Exemplo clássico

* Texto: `HELLOWORLD`
* Chave: `KEY`
* Saída (criptografado): `RIJVSUYVJN`

Como funciona (resumo)

A Vigenère desloca cada letra do texto claro por um valor derivado da **letra correspondente da chave**. Na prática, fazemos somas/ subtrações **módulo 26** (A…Z). Quando a chave acaba, ela **se repete** sobre o texto.

* **Criptografar**: `C = (P + K) mod 26`
* **Descriptografar**: `P = (C - K) mod 26`

Onde `P` é a letra do **Plaintext**, `C` do **Ciphertext**, e `K` o deslocamento definido pela **Key**.

---

## Referências para estudo

* Intro clássica: “Vigenère cipher” (Wikipedia)
* *The Code Book* — Simon Singh (capítulos sobre cifras históricas)
* Materiais de Segurança da Informação/Criptografia (anotações pessoais)

---

**PT**: Repo de estudo sobre criptografia clássica com foco na **cifra de Vigenère** em Python — para praticar conceitos, CLI e testes.
**EN**: Educational repo on classical cryptography focused on the **Vigenère cipher** in Python — to practice concepts, CLI usage, and testing.
