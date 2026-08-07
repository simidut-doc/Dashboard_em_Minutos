
<img width="1200" height="630" alt="titanic" src="https://github.com/user-attachments/assets/ebba5edf-ccd3-4ecd-8be1-22818943b8ef" />

# Dashboard_em_Minutos

# 📊 Dashboard em Minutos

> **Projeto prático** de um gerador de dashboards a partir de uma simples planilha de dados, usando IA para acelerar análise, geração de insights e tomada de decisão.
> 🏆 **Destaque:** Como subproduto, o projeto gera **duas versões** da mesma informação — um dashboard em **HTML** (interativo) e um em **PDF** (para compartilhamento) — permitindo escolher o melhor formato conforme a necessidade.

## 🎯 Objetivo do Projeto

Criar o **"Dashboard em Minutos"** no Claude para apoiar equipes na exploração e no manuseio de dados de qualquer assunto. A ferramenta analisa a base, identifica tendências, padrões e variações, define indicadores relevantes, gera insights e estrutura uma apresentação visual clara. O objetivo é transformar uma planilha crua em uma **fonte de informação clara e apresentável**, sem que o usuário precise lidar com uma montanha de dados brutos.

## 🚧 Contexto e Problema

Cansado de receber uma base de dados para analisar e não saber nem por onde começar? O "Dashboard em Minutos" resolve exatamente esse gargalo: transforma uma planilha em visualizações e insights prontos para discussão.

Nas empresas, as equipes lidam constantemente com diversas planilhas. Para quem está entrando no time ou mesmo para quem já está há mais tempo, isso pode ser desafiador — seja pela quantidade de assuntos, pela complexidade dos dados, pela dificuldade de interpretação, pela falta de conhecimento prévio sobre o tema ou simplesmente pela falta de tempo para uma análise cuidadosa. A ideia do projeto é **acelerar a curva de entendimento da base**, trazendo visões exploratórias com altíssima eficiência de tempo — daí o nome "em minutos".

## 🛠️ Tecnologias e IAs Utilizadas

- **[Claude (Sonnet 5)](https://claude.ai/):** Utilizado do planejamento à execução — elaboração do prompt base, definição das instruções do projeto e geração dos dashboards (HTML e PDF) a partir do arquivo anexado.

---

## 🗂️ Fontes de Dados

Para garantir que a IA traga informações precisas e não alucinadas, foi utilizada a seguinte base de dados pública:

| Fonte | Conteúdo / Finalidade | Tamanho |
| --- | --- | --- |
| **Titanic-Dataset.csv** ([Kaggle](https://www.kaggle.com/datasets/yasserh/titanic-dataset?select=Titanic-Dataset.csv)) | Dados de passageiros do RMS Titanic (idade, classe, tarifa, sobrevivência, etc.) | 61,19 KB (1 arquivo, 12 colunas) |

**🚀 Sobre esta base**

O naufrágio do Titanic é um dos mais infames da história. Em 15 de abril de 1912, durante sua viagem inaugural, o RMS Titanic — amplamente considerado "inafundável" — afundou após colidir com um iceberg. Não havia botes salva-vidas suficientes para todos a bordo, resultando na morte de 1.502 dos 2.224 passageiros e tripulantes.

Embora houvesse um elemento de sorte envolvido na sobrevivência, alguns grupos de pessoas tinham maior probabilidade de sobreviver do que outros. Que tipos de pessoas tinham maior chance de sobreviver? Essa é justamente a pergunta que o dashboard ajuda a responder de forma visual e rápida.

---

## 🚀 Passo a Passo da Construção

### Passo 1: Escolha da base de dados

Seleção do dataset no [Kaggle](https://www.kaggle.com/) — plataforma que disponibiliza conjuntos de dados públicos para estudos, pesquisas e projetos de ciência de dados.

### Passo 2: Engenharia de prompt (o coração do projeto)

Criação de um prompt detalhado no Claude, definindo:

- **Objetivo:** o que o dashboard deve entregar (indicadores, gráficos, insights).
- **Contexto:** o tipo de base que será analisada e o público-alvo do resultado.
- **Restrições:** não ser criativo com os números — trazer apenas dados precisos, extraídos diretamente do arquivo.
- **Tom/Estilo:** visual limpo, direto e orientado a decisão.

### Passo 3: Configuração do projeto no Claude

Criação de um projeto no Claude chamado **"Dashboard em Minutos"**, com as instruções acima registradas como conhecimento fixo do projeto (Project Instructions), garantindo que qualquer nova planilha anexada siga sempre o mesmo padrão de análise e saída.

### Passo 4: Execução

Dentro da área do projeto no Claude, basta anexar o arquivo na janela de chat e enviar o comando:

> *"Crie um dashboard a partir deste arquivo."*

O Claude analisa a planilha e entrega o dashboard já em dois formatos — HTML e PDF — prontos para uso.

---

## 💬 Guia de Prompts (Como explorar o projeto)

Alguns exemplos de comandos que podem ser usados dentro do projeto para ir além do dashboard padrão:

- *"Crie um dashboard a partir deste arquivo."*
- *"Quais variáveis têm maior correlação com a sobrevivência dos passageiros?"*
- *"Gere um dashboard focado apenas em idade e classe social."*
- *"Traga os principais outliers encontrados na base."*
- *"Resuma em 3 insights o que mais chama atenção nesses dados."*
- *"Exporte a mesma análise em versão PDF para envio por e-mail."*

### 🛡️ Testes Realizados

Para validar a robustez e os limites do projeto, foram feitos os seguintes testes:

- **Tamanho de arquivo:** testes com planilhas de diferentes tamanhos, funcionando de forma consistente com arquivos de até **XX MB** (ajustar conforme o maior arquivo validado).
- **Qualidade dos dados:** verificação de como o Claude lida com colunas com valores ausentes (ex: `Age` e `Cabin` no dataset do Titanic), confirmando que a ferramenta sinaliza a ausência em vez de estimar ou inventar valores.
- **Consistência entre formatos:** comparação entre a versão HTML e a versão PDF geradas a partir da mesma base, para garantir que os indicadores e números batem entre os dois formatos.

---

## 📌 Lições Aprendidas

1. **A qualidade do prompt define a qualidade do dashboard.** Prompts vagos geram análises genéricas; quanto mais claro o objetivo e as restrições, mais direto e útil é o resultado.
2. **Configurar o projeto no Claude (e não só o chat avulso) faz diferença.** Fixar as instruções no projeto garante padronização quando novas planilhas forem anexadas no futuro, sem precisar reescrever o prompt toda vez.
3. **Dois formatos de saída atendem públicos diferentes.** O HTML é melhor para exploração interativa; o PDF é melhor para compartilhar com quem só precisa do resultado final, sem interagir com os dados.

---

## 🙌 Agradecimentos

- **Instrutor MSc Grimaldo Lopes (Udemy)** por plantar a sementinha desta automação de IA.
- **Comunidade de IA e desenvolvimento** por todos os conhecimentos compartilhados.

---

## 👩‍💻 Autor

Feito com 💡 **Thais R. Garcia Simidu** e muita IA durante os estudos de Inteligência Artificial e Engenharia de Prompts.

---

**Última atualização:** Agosto de 2026
**Status:** ✅ Completo e pronto para exploração

---

## 🚀 Comece Agora!

- 👉 [Leia o Contexto e Objetivos](#-objetivo-do-projeto)
- 👉 [Explore a Fonte de Dados](#️-fontes-de-dados)
- 👉 Acesse o repositório: [Dashboard_em_Minutos](https://github.com/simidut-doc/Dashboard_em_Minutos)
