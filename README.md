# Projeto de Redes de Computadores 💻

Esse repositório contém um **Projeto de Redes de Computadores** construído em equipe para a disciplina de Redes de Computadores do Instituto de Computação, UFAL.

Um sistema de **chat em tempo real via socket TCP**, implementado em **Python**, com suporte a **vários clientes simultâneos**, **moderação automática** (palavras proibidas, avisos e banimentos), e **interface colorida no terminal** (via `colorama`).

---

## 🔧 Tecnologias usadas

**Linguagem:** Python  
**Ferramenta:** VS Code

---

## 🚀 Visão Geral

O projeto é composto por dois programas:

- **servidor.py** → gerencia conexões, mensagens e regras de moderação.  
- **cliente.py** → interface de chat no terminal para o usuário final.

Cada cliente se conecta ao servidor via **TCP (porta 55555, localhost por padrão)**.  
O servidor cria uma **thread dedicada** para cada cliente, recebendo mensagens, filtrando conteúdo e retransmitindo para todos os usuários conectados.

---

## 🛠️ Dependências

### Requisitos mínimos
- Python **3.8+**

### Bibliotecas padrão
- `socket`  
- `threading`  
- `sys`

### Dependência externa
```bash
pip install colorama
```

---

## 📁 Estrutura do Projeto

```
chat/
│
├── servidor.py     # Lado do servidor (controle, moderação, broadcast)
├── cliente.py      # Lado do cliente (envio e recebimento)
└── README.md       # Este documento
```

---

## ▶️ Como Rodar o Projeto

### 1️⃣ Inicie o servidor

Abra um terminal e execute:
```bash
python servidor.py
```

Você verá:
```
Servidor escutando em 127.0.0.1:55555
```

---

### 2️⃣ Conecte um cliente

Em outro terminal, execute:
```bash
python cliente.py
```

Informe seu apelido quando solicitado.  
Após conectar, você verá:
```
Conectado ao servidor!
```

---

## 📧 Contato

| Nome | E-mail |
|------|---------|
| Alexia Rodrigues Dos Santos Oliveira | arso@ic.ufal.br |
| Barbara Rocha de Albuquerque | bra@ic.ufal.br |
| Lara Nogueira Da Costa Ayres | lnca@ic.ufal.br |
| Leandro Marcio Elias da Silva | lmes@ic.ufal.br |
