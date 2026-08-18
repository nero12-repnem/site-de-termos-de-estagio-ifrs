# 📄 Gerador de Termo de Compromisso de Estágio

Sistema web desenvolvido para facilitar o preenchimento e a geração automática de **Termos de Compromisso de Estágio**.

O sistema possui um formulário organizado para coleta das informações da instituição, concedente e estagiário. Após o preenchimento, um documento é criado automaticamente no **Google Docs** e armazenado em uma pasta específica do **Google Drive**.

## 🚀 Funcionalidades

- Formulário web responsivo e organizado
- Dados institucionais do IFRS – Campus Alvorada
- Cadastro dos dados da concedente
- Cadastro dos dados do estagiário
- Verificação de maioridade
- Campo de responsável legal somente para menores de 18 anos
- Máscara automática para CPF
- Máscara automática para CNPJ
- Máscara para telefone
- Máscara para CEP
- Seleção de datas e horários
- Registro das atividades do estágio
- Geração automática do Termo de Compromisso
- Criação do documento no Google Docs
- Salvamento automático no Google Drive
- Link para acessar o documento após a geração

## 🛠️ Tecnologias utilizadas

- HTML5
- CSS3
- JavaScript
- Google Apps Script
- Google Docs API através do Apps Script
- Google Drive através do Apps Script

## ⚙️ Como funciona

O usuário preenche as informações necessárias através da interface web.

O `Index.html` coleta os dados e envia as informações para o Google Apps Script através de:

`google.script.run`

O arquivo `Code.gs` recebe os dados, monta o Termo de Compromisso e cria automaticamente um novo documento no Google Docs.

Depois da criação, o documento é enviado para uma pasta definida no Google Drive.

## 📁 Estrutura do projeto

    gerador-termo-estagio-ifrs/
    │
    ├── Code.gs
    ├── Index.html
    ├── README.md
    └── .gitignore

## 🌐 Hospedagem

A aplicação é publicada como um **Web App do Google Apps Script**.

Isso permite que o frontend se comunique diretamente com as funções do Apps Script responsáveis pela geração dos documentos.

## 🔒 Segurança

Dados sensíveis, credenciais, tokens e identificadores privados não devem ser armazenados diretamente no repositório público.

Ao utilizar este projeto, configure seus próprios recursos do Google Drive e as permissões necessárias no Google Apps Script.

## 📌 Objetivo

O projeto foi desenvolvido com o objetivo de tornar o processo de criação dos Termos de Compromisso de Estágio mais rápido, padronizado e simples, diminuindo a necessidade de preenchimento manual dos documentos.

## 👨‍💻 Autor

Desenvolvido por **Enzo da rosa severino**.

Projeto desenvolvido utilizando HTML, CSS, JavaScript e Google Apps Script.
