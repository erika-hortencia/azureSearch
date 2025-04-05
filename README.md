# azureSearch

Projeto que analisa comentários de clientes sobre uma loja de departamentos localizada em São Paulo utilizando Azure AI Search e Azure Cognitive Services. Os documentos foram armazenados em containers no Azure Blob Storage e processados para gerar insights sobre a experiência dos consumidores.

---

## 🛍️ Azure AI Search - Feedbacks de Clientes (Loja SP)

Este projeto demonstra como criar uma solução de *Knowledge Mining* com **Azure AI Search** e **Azure AI Services** para analisar avaliações reais/simuladas de clientes de uma loja de departamentos em São Paulo.

A solução permite extrair informações valiosas de documentos armazenados no Blob Storage, enriquecê-las com inteligência artificial e estruturá-las para pesquisa via índices.

---

## 📦 Tecnologias Utilizadas

- **Azure Blob Storage**: Armazena os documentos dos clientes em `.json`, `.txt` e `.docx`.
- **Azure AI Search**: Indexa os arquivos e aplica recursos de pesquisa textual, OCR e IA semântica.
- **Azure Cognitive Services**: Realiza extração de sentimento, localização, palavras-chave, identificação de entidades e tags de imagem.

---

## 🛠️ Passo a Passo: Como configurar a solução

Siga o tutorial completo da Microsoft para configuração do pipeline de AI Search: [aqui](https://microsoftlearning.github.io/mslearn-ai-fundamentals/Instructions/Labs/11-ai-search.html)


## 🔍 Exemplos de Consultas no Search Explorer

### Consultas básicas
```json
{
  "search": "*",
  "count": true
}
```
```json
{
  "search": "locations:'São Paulo'",
  "count": true
}
```
```json
{
  "search": "sentiment:'negative'",
  "count": true
}
```

### Consultas básicas
```json
{
  "search": "keyphrases:'atendimento'",
  "count": true
}
```
```json
{
  "search": "merged_content:'fila'",
  "count": true
}
```
```json
{
  "search": "merged_content:'variedade de produtos'",
  "count": true
}
```

---

## 🧠 Insights e Resultados
📊 Insight extraído da consulta: merged_content:'fila'
---

## ✅ Resumo dos resultados
A consulta retornou diversos documentos com menções negativas relacionadas a tempo de espera em filas, especialmente em horários de pico e finais de semana.

📍 Documento 1
Localização: São Paulo, SP

- Sentimento: Negativo

- Comentário: "Fui atendido após mais de 30 minutos na fila. A loja estava cheia e não havia organização no setor de eletrônicos."

- Insight: Problema recorrente que pode ser solucionado com reforço de equipe em horários de pico.

📍 Documento 2
Localização: São Paulo, SP

- Sentimento: Positivo

- Comentário: "Mesmo com a loja cheia, percebi que o caixa rápido foi eficiente e agilizou a fila."

- Insight: Os caixas rápidos são bem avaliados e podem ser expandidos para outros setores.

---

## 💡 Conclusão dos insights
O sentimento predominante gira em torno da experiência de atendimento, agilidade no caixa, organização da loja e disponibilidade de produtos.

As ferramentas de IA da Azure mostraram-se eficazes para processar linguagem natural e gerar insights acionáveis a partir de feedbacks textuais.

A análise pode embasar melhorias operacionais, ações de marketing e atendimento ao cliente.

---

## 📚 Aprendizados Adquiridos
Estruturação de um pipeline completo de análise com Azure AI Search.

Indexação e enriquecimento de dados não estruturados com IA.

Criação de queries para explorar sentimentos, entidades e padrões nos dados.

Compreensão de como usar IA para otimizar a experiência do cliente no varejo.
