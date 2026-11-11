# Python + Google Sheets com Apps Script

Este projeto envia e consulta mensagens (contendo nome e e-mail) em uma planilha do Google. A integração funciona utilizando o Google Apps Script como uma pequena API web.

## 🚀 Funcionalidades

O notebook está dividido em operações de envio (POST) e consulta (GET):

* **`enviar_mensagem(nome, email)`**: Envia uma única mensagem para a planilha e imprime o texto de confirmação de sucesso do servidor.
* **`enviar_varias_mensagens(mensagens)`**: Recebe uma lista de dicionários com mensagens e envia uma por vez.
* **`obter_todas_mensagens()`**: Busca todas as mensagens da planilha e as exibe em formato JSON legível, utilizando os cabeçalhos da planilha (Data, Nome, Email) como chaves.
* **`obter_ultima_mensagem()`**: Retorna apenas a última mensagem registrada, ou exibe um aviso caso não haja nenhuma.

## 🛠️ Tecnologias Utilizadas

* **Python 3** (via Google Colab).
* **`requests`**: Biblioteca utilizada para realizar as requisições HTTP (POST e GET).
* **`json`**: Biblioteca utilizada para formatar e exibir as respostas de forma legível na tela.

## ⚙️ Como Configurar e Usar

1. **Ambiente:** Abra o notebook no Google Colab. Não é necessário instalar bibliotecas externas, pois o Colab já traz o Python e a biblioteca `requests` nativamente.
2. **Configuração da API:** Localize a variável `API_URL` na primeira célula de código. Substitua o valor padrão pela URL da sua própria implantação do Apps Script (a URL deve terminar com `/exec` e iniciar com `https://script.google.com/`) mantendo as aspas
3. **Execução:** Execute as células sequencialmente de cima para baixo, usando o botão de *play* ao lado esquerdo de cada célula ou o atalho `Shift + Enter`.

---
*Sinta-se à vontade para explorar o código, abrir issues ou enviar pull requests caso queira contribuir para o projeto!*
