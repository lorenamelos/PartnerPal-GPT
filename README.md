# PartnerPal: Um Chatbot com Inteligência Emocional 💞

## Visão Geral

PartnerPal é um chatbot baseado em IA projetado para simular conversas emocionalmente inteligentes entre parceiros. Ele utiliza modelos avançados de NLP para detectar emoções e sentimentos no texto do usuário e responder de forma empática e compreensiva. Este projeto demonstra a integração de modelos de análise de emoção e sentimento com um modelo de linguagem de grande porte para criar um chatbot altamente interativo e ciente do contexto.


## Funcionalidades

- **Detecção de Emoção e Sentimento**: O chatbot usa modelos `DistilBERT` para prever as emoções e sentimentos do usuário. Essas previsões orientam as respostas, garantindo que sejam contextualmente apropriadas e emocionalmente ressonantes.
  
- **Aprendizado por Exemplos (Few-Shot Learning)**: O chatbot incorpora exemplos pré-definidos na construção das respostas para manter um estilo e tom consistentes na conversa.

- **Geração de Respostas em Tempo Real**: As respostas são geradas de forma contínua e interativa, melhorando a experiência do usuário.

- **Integração com OpenAI API**: PartnerPal usa a API da OpenAI para acessar o modelo `GPT-4o-mini`, que gera as respostas do chatbot de forma eficiente e escalável.

## Modelos Utilizados

1. **Modelo de Detecção de Emoções**: [`bhadresh-savani/distilbert-base-uncased-emotion`](https://huggingface.co/bhadresh-savani/distilbert-base-uncased-emotion)
2. **Modelo de Análise de Sentimentos**: [`distilbert-base-uncased-finetuned-sst-2-english`](https://huggingface.co/distilbert/distilbert-base-uncased-finetuned-sst-2-english)
3. **Modelo de Linguagem**: `GPT-4o-mini` via [OpenAI API](https://openai.com/research/gpt-4)

## Como Funciona

1. **Entrada do Usuário**: O usuário interage com o chatbot pela interface Streamlit.
2. **Análise de Emoção e Sentimento**: A entrada é processada por modelos de NLP da Hugging Face para detectar emoções e sentimentos.
3. **Geração de Resposta**: O chatbot gera uma resposta usando `GPT-4o-mini`, considerando exemplos pré-definidos e o histórico da conversa.
4. **Interação Contínua**: O chatbot mantém o contexto e adapta suas respostas com base nas emoções detectadas.

## Requisitos

- `torch`
- `transformers`
- `streamlit`
- `openai`

## Configuração

1. Clone este repositório:
    ```bash
    git clone https://github.com/seuusuario/PartnerPal.git
    cd partnerpal
    ```

2. Instale as dependências:
    ```bash
    pip install -r requirements.txt
    ```

3. Execute a aplicação Streamlit:
    ```bash
    streamlit run PartnerPal.py
    ```

## Trabalhos Futuros

- **Aprimoramento da Compreensão Contextual**: Melhorar o entendimento de emoções complexas e sentimentos sutis.
- **Memória Multi-Turno**: Expandir a capacidade do chatbot de lembrar conversas entre sessões.
- **Aprimoramento da Memória de Conversação**: Tornar o chatbot mais capaz de reter o contexto e oferecer respostas mais personalizadas.

## Agradecimentos

- **OpenAI API**: Obrigado à equipe OpenAI por fornecer acesso ao `GPT-4o-mini`. Saiba mais sobre o modelo [aqui](https://openai.com/research/gpt-4).
- **Hugging Face**: Agradecimento especial ao Hugging Face por fornecer modelos pré-treinados para análise de emoção e sentimentos. Confira o modelo de detecção de emoções [aqui](https://huggingface.co/bhadresh-savani/distilbert-base-uncased-emotion) e o modelo de análise de sentimentos [aqui](https://huggingface.co/distilbert/distilbert-base-uncased-finetuned-sst-2-english).

## Licença

Este projeto é licenciado sob a Licença MIT. Veja o arquivo [LICENSE](LICENSE) para mais detalhes.

### Licenças dos Modelos

1. **Modelo de Análise de Sentimentos DistilBERT**: Licenciado sob a Licença Apache 2.0. Veja detalhes [aqui](https://huggingface.co/distilbert/distilbert-base-uncased-finetuned-sst-2-english/discussions).
2. **OpenAI API**: O uso da API está sujeito aos termos da OpenAI. Consulte a [documentação oficial](https://openai.com/research/gpt-4) para mais informações.



