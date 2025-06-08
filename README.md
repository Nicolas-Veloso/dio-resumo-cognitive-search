# dio-resumo-cognitive-search
---
## Guia Básico: Configurando um Projeto com Azure Cognitive Search

---

### Passo 1: Criar um Serviço de Azure Cognitive Search

1. Acesse o portal do Azure: [https://portal.azure.com](https://portal.azure.com)  
2. Clique em **Criar um recurso**.  
3. Pesquise por **Azure Cognitive Search** e clique para criar.  
4. Preencha:  
   - Nome do serviço  
   - Região  
   - Plano de preço (comece com a camada gratuita, se disponível)  
5. Clique em **Criar** e aguarde a implantação.

---

### Passo 2: Preparar os Dados para Indexação

- Utilize uma fonte de dados, como:  
  - Blob Storage do Azure com documentos (JSON, PDF, TXT, etc.)  
  - Banco de dados SQL  
  - Cosmos DB  
  - Outros suportados

---

### Passo 3: Criar um Índice

- O índice define os campos pesquisáveis, filtráveis, etc.  
- Exemplo simples de campos do índice:  
  - `id` (string, chave)  
  - `title` (string, pesquisável)  
  - `content` (string, pesquisável)  
  - `createdDate` (date, filtrável)  

- Pode ser criado via Portal Azure, SDKs ou REST API.

---

### Passo 4: Criar um Data Source (Fonte de Dados)

- Configure a conexão com o armazenamento (ex: Blob Storage).  
- Defina o container ou tabela que será usada.

---

### Passo 5: Criar um Indexer

- O indexer lê a fonte de dados e popula o índice.  
- Configure a frequência para atualizar o índice automaticamente.

---

### Passo 6: Realizar Consultas

- Execute consultas simples ou complexas via SDK, REST API ou Portal.  
- Exemplos:  
  - Buscar termos específicos  
  - Filtrar resultados  
  - Ordenar por data

---

### Passo 7 (Opcional): Usar Recursos de IA para Enriquecer Dados

- Configure **skillsets** com recursos de IA, como:  
  - Extração de frases-chave  
  - OCR (Reconhecimento ótico de caracteres)  
  - Tradução automática  

- Isso enriquece seus documentos para buscas mais inteligentes.

