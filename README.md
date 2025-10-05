# 🚌 Consulta de Rotas de Ônibus com Python

![Python](https://img.shields.io/badge/Python-3.7%2B-blue.svg?style=for-the-badge&logo=python)
![APIs do Google](https://img.shields.io/badge/Google_Routes_API-4285F4?style=for-the-badge&logo=google)

Um script em Python que utiliza a API do Google Routes para encontrar a próxima partida de ônibus entre dois pontos, ideal para descobrir horários e planejar viagens de transporte público.

---

## 📜 Sobre o Projeto

Este projeto demonstra como consumir APIs RESTful do Google usando Python, com foco em obter informações práticas do dia a dia. O objetivo é fornecer uma ferramenta de linha de comando leve e fácil de usar para consultar rotas de ônibus, mostrando informações essenciais como linha, parada e horários de partida e chegada.

É um ótimo exemplo para iniciantes em Python que desejam aprender a:
* Fazer requisições a uma API REST com a biblioteca `requests`.
* Lidar com dados no formato JSON.
* Configurar e usar chaves de API do Google Cloud de forma segura.
* Criar scripts Python reutilizáveis e bem estruturados.

---

## ✨ Funcionalidades

* **Busca de Rotas:** Encontra rotas de ônibus entre um endereço de origem e um de destino.
* **Informações Detalhadas:** Retorna o nome da linha, parada de partida, horário de partida, parada de chegada e horário previsto de chegada.
* **Fácil Configuração:** Todas as variáveis (chave de API, origem, destino) estão centralizadas no topo do script para fácil edição.
* **Tratamento de Erros:** Exibe mensagens de erro claras da API do Google em caso de falhas (ex: chave inválida, rota não encontrada, erro de conexão).

---

##  Como Usar

Para executar este script, siga os passos abaixo.

### Pré-requisitos

1.  **Python 3:** Você precisa ter o Python 3 instalado. Para verificar, abra seu terminal e digite `python --version` ou `py --version`.
2.  **Biblioteca `requests`:** Esta biblioteca é usada para fazer as chamadas de API.

### Configuração

1.  **Clone ou baixe este repositório.**

2.  **Crie sua Chave de API:**
    * Acesse o [Google Cloud Console](https://console.cloud.google.com/).
    * Crie um novo projeto.
    * Ative a **"Routes API"** para o projeto.
    * Vincule uma **conta de faturamento** (o Google oferece um nível de uso gratuito generoso).
    * Vá para "Credenciais", crie uma "Chave de API" e restrinja-a para permitir apenas o uso da "Routes API".

3.  **Instale as dependências:**
    * Abra seu terminal na pasta do projeto e instale a biblioteca `requests` com o pip:
      ```bash
      pip install requests
      ```

4.  **Edite o Script (`consulta_onibus.py`):**
    * Abra o arquivo `.py` em um editor como o VS Code.
    * Localize a seção `# --- CONFIGURAÇÃO ---` no topo do arquivo.
    * Preencha as variáveis com suas informações:
        ```python
        # 1. Cole aqui a sua Chave de API do Google Cloud.
        API_KEY = ""

        # 2. Defina o endereco de partida.
        ORIGEM = "Avenida Paulista, 1578, São Paulo, Brasil"

        # 3. Defina o endereco de destino.
        DESTINO = "Parque Ibirapuera, São Paulo, Brasil"
        ```

### Execução

1.  Abra seu **terminal** (PowerShell, CMD, Git Bash, etc.).
2.  Navegue até a pasta onde você salvou o script:
    ```bash
    cd C:\Caminho\Para\O\Seu\Projeto
    ```
3.  Execute o script usando o comando `python`:
    ```bash
    python consulta_onibus.py
    ```
A saída com os detalhes da rota de ônibus aparecerá no terminal.

---

## 📄 Licença

Este projeto é distribuído sob a licença MIT. Veja o arquivo `LICENSE` para mais detalhes.
