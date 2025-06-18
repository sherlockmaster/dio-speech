# 🚀 Desafio DIO: Laboratório Azure Speech Studio & Language Studio

Este repositório documenta minha experiência e aprendizados durante o laboratório prático da DIO para uso do Azure Speech Studio e Language Studio, explorando IA para análise de fala e linguagem natural.

## 📍 Sumário

- [Descrição do Desafio](#descrição-do-desafio)
- [Ferramentas Utilizadas](#ferramentas-utilizadas)
- [Experiência Prática e Etapas](#experiência-prática-e-etapas)
    - [1. Speech Studio](#1-speech-studio)
    - [2. Language Studio](#2-language-studio)
- [Principais Aprendizados](#principais-aprendizados)
- [Dificuldades e Soluções](#dificuldades-e-soluções)
- [Capturas de Tela](#capturas-de-tela)
- [Referências](#referências)

---

## Descrição do Desafio

Praticar o uso de IA aplicada à voz e linguagem natural no Azure, com foco nas ferramentas Speech Studio e Language Studio, desenvolvendo experimentos, analisando resultados e documentando toda a jornada.

---

## Ferramentas Utilizadas

- [Azure Speech Studio](https://speech.microsoft.com/)
- [Azure Language Studio](https://language.cognitive.azure.com/)
- Conta de avaliação gratuita no Azure
- Navegador Google Chrome

---

## Experiência Prática e Etapas

### 1. **Speech Studio**

#### 1.1 Criação do recurso
- Acesse o portal do Azure, clique em **"Criar recurso"** e pesquise por *Speech*.
- Complete a configuração (nome, região, tipo de preço F0 para testes).
- Recurso criado com sucesso! Veja a tela inicial:

![Speech Portal](images/speech-portal.png)

#### 1.2 Reconhecimento de Fala (Speech to Text)
- Acesse o menu *Speech Studio* e escolha **"Transcrição de fala"**.
- Fiz upload de um áudio curto: “Olá, mundo! Estou testando o reconhecimento de fala.”
- Resultado automático exibido rapidamente:
    - Texto transcrito: *"Olá, mundo! Estou testando o reconhecimento de fala."*
    - Veja o exemplo de tela:

![Transcrição](images/speech-transcription.png)

#### 1.3 Síntese de Fala (Text to Speech)
- Digitei o texto: “Inteligência artificial no Azure é poderosa!”.
- Escolhi a voz `pt-BR-FranciscaNeural` e baixei o áudio. A qualidade é bastante natural.
- Playground de sintonia permite ajustar entonação e velocidade da fala.

#### 1.4 Customização de Modelos
- Testei carregar um pequeno dataset de amostras de áudio próprios como experimento. Exige mais dados para resultados relevantes, mas entendi todo o fluxo de customização.

---

### 2. **Language Studio**

#### 2.1 Criação do recurso
- Mesma lógica do Speech Studio: Criei um *Language Resource*.
- Dashboard intuitivo para testes.

#### 2.2 Análise de Sentimento
- Testei o texto: "Estou muito satisfeito com o serviço, parabéns!"
- Resultado (score): **Positivo** (score 0.97)
- Resultado visual:

![Sentimento](images/language-sentiment.png)

#### 2.3 Extração de Entidades
- Texto usado: "Bill Gates fundou a Microsoft em 1975 em Albuquerque."
- Entidades extraídas:
    - **Pessoa**: Bill Gates
    - **Organização**: Microsoft
    - **Data**: 1975
    - **Localização**: Albuquerque

![Entidades](images/language-entities.png)

#### 2.4 Detecção de idioma e key phrases
- Testei textos em inglês e português e foi detectado corretamente.
- Key phrases destacadas automaticamente pelo modelo.

---

## Principais Aprendizados

- Azure Speech Studio oferece recursos abrangentes e simples de usar para transcrição de áudio, síntese de fala e personalização de modelos.
- Language Studio permite análise avançada de textos, incluindo sentimento, entidades, idioma e frases chave.
- A integração das duas ferramentas é útil para aplicações focadas em acessibilidade, inteligência comercial, chatbots e automação de atendimentos.

---

## Dificuldades e Soluções

| Dificuldade                                    | Solução Adotada                                                                    |
|------------------------------------------------|------------------------------------------------------------------------------------|
| Recursos demorando para serem criados no Azure | Aguardei alguns minutos e atualizei a dashboard; normalmente leva até 5 minutos.   |
| Áudio longo não funcionando                    | Limitei os uploads para < 1 minuto nos testes gratuitos.                           |
| Erro de permissão na API                       | Revisei as chaves de acesso do recurso e redefini as permissões no portal.         |

---

## Capturas de Tela

As imagens dos principais experimentos estão na pasta [`/images`](images/).

---

## Referências

- [Documentação Speech Studio](https://learn.microsoft.com/pt-br/azure/ai-services/speech-service/)
- [Documentação Language Studio](https://learn.microsoft.com/pt-br/azure/ai-services/language-service/)
- [Laboratório Speech Studio - Microsoft Learning](https://learn.microsoft.com/pt-br/training/modules/explore-speech-studio/)
- [Laboratório Language Studio - Microsoft Learning](https://learn.microsoft.com/pt-br/training/modules/analyze-text-language-studio/)

---

## 📢 Conclusão

Esse laboratório demonstrou, na prática, o que é possível fazer combinando inteligência artificial de voz e linguagem no Azure. Reforço que tanto para aplicações comerciais quanto educacionais, é uma abordagem acessível para acelerar resultados!

Dúvidas ou sugestões? Fique à vontade para abrir Issues ou Pull Requests.
