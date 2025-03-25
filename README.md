# Projeto - Pesquisa com Azure AI Search 
**Nesse projeto eu realizo a organização de documentos e pesquisa eficiente com Azure AI Search, como proposto no desafio da DIO**

# Objetivo  
Demonstrar **ingestão de dados**, **criação de índices** e **exploração de funcionalidades** do Azure AI Search usando apenas a interface do Azure.  


# **Passo a Passo Visual**  

 **1. Ingestão de Dados**  
**Exemplo**:  
- Dados usados (simulados):  
---
id,titulo,conteudo,categoria  
1,O Impacto do 5G no IoT,"A combinação de 5G e IoT está criando cidades inteligentes mais eficientes...",Tecnologia  
2,Análise de Dados com Pandas,"Domine técnicas avançadas de análise de dados usando Pandas e Python...",Data Science  
3,Blockchain além das Criptomoedas,"Como a tecnologia blockchain está sendo aplicada em supply chain e saúde...",Inovação
---
# **Como fazer:**

- Acesse o Portal Azure.

- No serviço Azure AI Search, clique em "Importar dados".

- Selecione a fonte (ex: um arquivo CSV fictício como o acima).

- Importar Dados

# **2. Criação do Índice**

Durante a importação, o Azure gera automaticamente o índice.

# **3. Exploração das Funcionalidades**
**Exemplo de buscas:**

**Texto livre:**
**"5G" →** Retorna documentos que mencionam "5G" no título ou conteúdo (como o artigo sobre IoT).

**Filtro:**
categoria eq 'Data Science' → Mostra só artigos de análise de dados.

**Combinados:**
search="Python" AND filter="categoria eq 'Data Science'" → Encontra o artigo sobre Pandas que menciona Python.


# Insights e Aprendizados
**Ferramentas que se beneficiam:**

- Bases de conhecimento internas (ex: FAQs de suporte técnico).

- Catálogos de produtos (e-commerce).

**Destaques do Azure AI Search:**

**Facets:** Permite refinamento por categorias.

**Sinônimos:** Busca por "computador" também acha "PC".
