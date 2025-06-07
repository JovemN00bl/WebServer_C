# Web Server Simples em C

![Status](https://img.shields.io/badge/status-funcional-green)
![Linguagem](https://img.shields.io/badge/linguagem-C-blue)
![Plataforma](https://img.shields.io/badge/plataforma-Linux-orange)

Um web server HTTP minimalista desenvolvido em C, projetado para rodar em sistemas Linux. Este projeto demonstra os fundamentos da programação de sockets (`socket`, `bind`, `listen`, `accept`) para criar um servidor que escuta na porta **8080** e responde a todas as requisições com uma página HTML estática.

<br>

## ✨ Funcionalidades

-   **Servidor HTTP Básico:** Responde a requisições GET com uma resposta `HTTP/1.1 200 OK`.
-   **Página Estática:** Serve uma página HTML simples com a mensagem "Hello World!".
-   **Loop Infinito:** O servidor continua em execução, aceitando novas conexões indefinidamente.
-   **Socket Reutilizável:** Configurado com `SO_REUSEADDR`, permitindo que o servidor seja reiniciado rapidamente sem aguardar a liberação da porta.

---

## 🛠️ Tecnologias Utilizadas

-   **Linguagem:** C
-   **APIs e Bibliotecas:**
    -   Programação de Sockets Linux (`sys/socket.h`, `arpa/inet.h`)
    -   Bibliotecas Padrão do C (`stdio.h`, `stdlib.h`, `string.h`, `unistd.h`)

---



## 🌐 Como Testar

Após iniciar o servidor, você pode testá-lo de duas maneiras:

1.  **Pelo Navegador:**
    -   Abra qualquer navegador web (Chrome, Firefox, etc.).
    -   Acesse a URL: **http://localhost:8080**

2.  **Pelo Terminal (usando `curl`):**
    -   Abra um novo terminal.
    -   Execute o seguinte comando:
    ```bash
    curl http://localhost:8080
    ```

Em ambos os casos, você deverá ver a página HTML "Hello World!" sendo retornada pelo servidor. Para parar o servidor, volte ao terminal onde ele está rodando e pressione `Ctrl + C`.
