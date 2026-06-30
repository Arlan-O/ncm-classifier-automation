# Classificador Automático de NCM
Automação desenvolvida para reduzir o tempo de classificação fiscal de produtos utilizando regras de NCM e integração com APIs REST. O fluxo processa listas em lote, realiza consultas automáticas, aplica regras de classificação e registra os resultados em uma planilha do Google Sheets.

## 🚀 Tecnologias

<p align="left">
  <img src="https://img.shields.io/badge/n8n-EA4B71?style=for-the-badge&logo=n8n&logoColor=white" alt="n8n"/>
  <img src="https://img.shields.io/badge/API_REST-02569B?style=for-the-badge&logo=fastapi&logoColor=white" alt="API REST"/>
  <img src="https://img.shields.io/badge/JavaScript-F7DF1E?style=for-the-badge&logo=javascript&logoColor=black" alt="JavaScript"/>
  <img src="https://img.shields.io/badge/HTTP_Request-4A90E2?style=for-the-badge&logo=postman&logoColor=white" alt="HTTP Request"/>
  <img src="https://img.shields.io/badge/Google_Sheets-34A853?style=for-the-badge&logo=googlesheets&logoColor=white" alt="Google Sheets"/>
</p>

## ✨ Principais funcionalidades

- Processamento em lote de aproximadamente 750 códigos NCM
- Consulta automática 
- Aplicação de regras de classificação fiscal
- Tratamento e normalização das respostas
- Registro automático dos resultados no Google Sheets
- Fluxo desenvolvido inteiramente em n8n

## 💡 Desafios

- Tratamento de respostas inconsistentes da API
- Produtos com múltiplas classificações possíveis
- Organização do fluxo para processamento em lote
- Garantia de desempenho durante consultas em massa

## Como funciona

1. Recebe uma lista de NCMs de produtos em uma planilha do Google Sheets.
2. Consulta uma planilha com regras de classificação.
3. Processa a resposta.
4. Retorna possíveis classificações (o mesmo NCM pode ter mais de uma classificação dependendo da finalidade).
5. Grava os resultados em uma planilha.
6. A última validação deve ser feita pelo contador.


## Demonstração

### Fluxo

<img width="1492" height="702" alt="Group 271" src="https://github.com/user-attachments/assets/471c25d9-ed18-470f-bb5a-0ca70fae95ca" />

##

### Lista de NCMs para serem classificados, uma lista com aproximadamente 750 NCMs

<img width="350" height="719" alt="image" src="https://github.com/user-attachments/assets/0b202ceb-dd20-422a-9d1f-a9bf8d3f2d8f" />

##

### Planilha de regras

<img width="1643" height="720" alt="image" src="https://github.com/user-attachments/assets/81d3b16d-5476-43eb-b352-2e4bef8e2379" />

##

### Planilha após a classificação

<img width="1832" height="650" alt="image" src="https://github.com/user-attachments/assets/9dfcbf16-c96f-40c5-bb7a-04393d685448" />

##

## Observação

O fluxo do n8n não foi disponibilizado publicamente por conter regras de negócio específicas. Entretanto, o funcionamento da solução é demonstrado pelas imagens e pela documentação deste projeto.


