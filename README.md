# 
# Sistema de Criação de Posts para Instagram com Agentes de IA

Projeto da Imersão IA Alura + Google Gemini

Este projeto foi desenvolvido durante a Imersão IA da Alura em parceria com o Google, com foco na criação de um sistema automatizado de geração de posts para redes sociais (ex: Instagram) utilizando modelos Gemini e agentes inteligentes.
## Objetivo

O objetivo é construir um pipeline de 4 agentes de IA cooperativos, que trabalham em sequência para gerar, revisar e entregar posts otimizados para redes sociais.
Cada agente desempenha uma função específica, permitindo uma automação criativa e estruturada.
| Agente   | Nome                            | Função                                                       | Modelo                         |
| -------- | ------------------------------- | ------------------------------------------------------------ | ------------------------------ |
| 🕵️‍♂️ 1 | **Agente Buscador de Notícias** | Busca informações recentes e relevantes sobre o tópico.      | `gemini-2.0-flash`             |
| 🧩 2     | **Agente Planejador de Posts**  | Cria um plano de conteúdo com base nas notícias encontradas. | `gemini-2.0-flash`             |
| ✍️ 3     | **Agente Redator**              | Gera um rascunho de post engajador para o Instagram.         | `gemini-2.5-pro-preview-03-25` |
| 🔍 4     | **Agente Revisor de Qualidade** | Avalia o texto final, revisando clareza, tom e engajamento.  | `gemini-2.5-pro-preview-03-25` |

## Tecnologias utilizadas

• Python 3

• Google Colab

• Google Gemini SDK (google-genai)

• Google ADK (Agent Development Kit)

• Ferramenta de busca integrada (google_search)

Bibliotecas auxiliares:

• requests

• datetime

• IPython.display

• textwrap
## Instalação

Instalar dependências

No Google Colab ou ambiente local:

```bash
pip install google-genai google-adk

```
Configurar a chave da API

No Colab:

```bash
from google.colab import userdata
os.environ["GOOGLE_API_KEY"] = userdata.get('GOOGLE_API_KEY')
```
    
## Como funciona

• O usuário informa um tópico de interesse (ex: “Inteligência Artificial na Educação”);

• O Agente Buscador procura notícias recentes sobre o tema;

• O Agente Planejador organiza um plano de conteúdo com base nessas notícias;

• O Agente Redator escreve um post criativo e otimizado para o Instagram;

• O Agente Revisor verifica a qualidade final e faz sugestões de melhoria.

No final, o sistema entrega:

✅ Um post completo pronto para publicação.

✅ Um fluxo automatizado e modular para criação de conteúdo.


## Roadmap 

- Finalizar a implementação dos parâmetros dos agentes.

- Integrar o sistema com redes sociais (API do Instagram).

- Criar interface web (ex: Streamlit ou Gradio).

- Adicionar logs e histórico de execução.
## Referência

 - Imersão IA Alura + Google Gemini
