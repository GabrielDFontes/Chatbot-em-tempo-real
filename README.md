# Chatbot com IA em Tempo Real

Este projeto consiste no desenvolvimento de um chatbot com Inteligência Artificial, utilizando Python, Streamlit e a API do Google Gemini. A aplicação permite que o usuário envie mensagens e receba respostas geradas pela IA em uma interface interativa, mantendo o histórico da conversa durante a utilização.

## Tecnologias utilizadas

* **Python**
* **Streamlit** — criação da interface web interativa.
* **OpenAI Python SDK** — biblioteca utilizada para realizar a comunicação com a API do Gemini por meio de sua interface compatível com a OpenAI.
* **Google Gemini API** — responsável pela geração das respostas da inteligência artificial.

## Funcionalidades

* Envio de mensagens pelo usuário.
* Geração de respostas com Inteligência Artificial.
* Exibição das mensagens do usuário e da IA na interface.
* Armazenamento do histórico da conversa durante a sessão.
* Interface simples e interativa.

## Instalação e configuração

### 1. Instalar o Python

Instale o Python no computador, caso ainda não esteja instalado.

### 2. Instalar as bibliotecas

Abra o **CMD (Prompt de Comando)** e execute:

```bash
pip install openai streamlit
```

Após concluir a instalação, **reinicie o computador**.

### 3. Obter a chave da API do Gemini

Para utilizar a inteligência artificial, é necessário obter uma chave de API do Google Gemini.

1. Acesse o [Google AI Studio](https://aistudio.google.com/).
2. Entre na sua conta Google.
3. Acesse a área de gerenciamento de chaves de API (*API keys*), pelo painel ou dashboard.
4. Selecione a opção para **criar uma chave de API**.
5. Escolha ou crie um projeto Google e defina um nome para identificá-lo.
6. Copie a chave gerada e guarde-a em um local seguro.

### 4. Configurar a chave de API

No arquivo `main.py`, localize o trecho que inicializa o cliente:

```python
modelo = OpenAI(
    api_key="SUA_CHAVE_AQUI",
    base_url="https://generativelanguage.googleapis.com/v1beta/openai"
)
```

Substitua `SUA_CHAVE_AQUI` pela chave de API obtida no Google AI Studio.

### 5. Executar o projeto

Abra o CMD ou o terminal do VS Code na pasta em que está localizado o arquivo `nome_do_arquivo.py`.

Execute o seguinte comando:

```bash
streamlit run nome_do_arquivo.py
```

O Streamlit iniciará a aplicação e exibirá um endereço local no terminal. Abra esse endereço no navegador para utilizar o chatbot.

## Como utilizar

1. Abra a aplicação no navegador.
2. Digite uma mensagem no campo de texto.
3. Envie a mensagem.
4. Aguarde a resposta gerada pela IA.
5. Continue a conversa: as mensagens anteriores ficam armazenadas no histórico da sessão.

## Estrutura do projeto

```text
chatbot-ia-tempo-real/
├── nome_do_arquivo.py
├── README.md
├── requirements.txt
└── .gitignore
```

* `nome_do_arquivo.py`: contém o código principal do chatbot.
* `README.md`: apresenta a documentação do projeto.
* `requirements.txt`: lista as bibliotecas necessárias.
* `.gitignore`: define os arquivos e diretórios que não devem ser enviados ao GitHub.

## Dependências

O projeto utiliza as seguintes bibliotecas Python:

```text
streamlit
openai
```

## Autor

Projeto acadêmico desenvolvido para estudo e prática de programação com Inteligência Artificial.
