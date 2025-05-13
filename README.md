# 🧠 Laboratório Azure: Speech Studio e Language Studio

## 🎯 Objetivo

Este laboratório teve como foco explorar as ferramentas **Azure Speech Studio** e **Azure Language Studio** para desenvolver habilidades práticas em **análise de fala** e **linguagem natural (NLP)**. A proposta é utilizar serviços de inteligência artificial da Microsoft para transformar voz em texto, entender significado, sentimentos e entidades em linguagem natural.

---

## 🗂️ Estrutura do Repositório

| Pasta/Arquivo                        | Descrição                                                  |
|-------------------------------------|------------------------------------------------------------|
| `speech-studio/anotacoes-speech.md` | Notas e comandos sobre reconhecimento de fala              |
| `language-studio/anotacoes-language.md` | Dicas e práticas sobre análise de texto, sentimentos, etc. |
| `exemplos/`                          | Exemplos de transcrição e análise semântica                |
| `imagens/`                           | Capturas de tela da interface e resultados (opcional)      |

---

## 🔊 Azure Speech Studio

### Funcionalidades Exploradas:
- Conversão de voz para texto (Speech-to-Text)
- Personalização de modelos acústicos
- Geração de voz sintética (Text-to-Speech)
- Exportação em JSON com timestamp

📄 Veja mais em [`speech-studio/anotacoes-speech.md`](./speech-studio/anotacoes-speech.md)

---

## 🧾 Azure Language Studio

### Funcionalidades Exploradas:
- Análise de sentimentos
- Extração de entidades (NER)
- Classificação de texto
- Tradução e detecção de idioma

📄 Detalhes em [`language-studio/anotacoes-language.md`](./language-studio/anotacoes-language.md)

---

## 💡 Exemplos Incluídos

- ✅ `transcricao-audio.txt`: Resultado da conversão de um áudio gravado para texto.
- ✅ `analise-entidades.json`: Exemplo da estrutura de resposta de análise semântica.

---

## 📌 Conclusão

O uso das ferramentas **Speech Studio** e **Language Studio** permite desenvolver soluções práticas e poderosas com base em IA, como bots conversacionais, sistemas de transcrição, assistentes de voz e análises de texto em larga escala.

Este repositório serve como referência prática para novos projetos utilizando **Azure Cognitive Services**.

---

📅 **Data**: Maio de 2025  
👤 **Autor**: Marcio

# 🗣️ Azure Speech Studio – Anotações e Dicas

## 🎯 Objetivo
Explorar os recursos de conversão de fala em texto (Speech-to-Text) e texto em fala (Text-to-Speech), além da personalização de voz com modelos próprios.

---

## 🔹 Reconhecimento de Fala (Speech-to-Text)

### Passos:
1. Acesse [speech.microsoft.com](https://speech.microsoft.com)
2. Vá em **Speech-to-Text** > **Custom Speech**.
3. Faça upload de um arquivo `.wav` ou `.mp3`.
4. Execute o processo de transcrição.
5. Visualize os resultados com timestamps por palavra.

### 🔍 Dicas:
- Utilize arquivos com **boa qualidade de áudio** e sem ruídos.
- Habilite **diarização** se houver múltiplos falantes.
- Exporte em **JSON** para uso em sistemas externos.

---

## 🔸 Síntese de Fala (Text-to-Speech)

### Passos:
1. Vá em **Text-to-Speech**.
2. Escreva uma frase e escolha uma **voz neural** (ex: "pt-BR-AntonioNeural").
3. Escute, ajuste entonação, pausa e exporte o áudio em `.mp3`.

### 💡 Dicas:
- Use **SSML** para controle refinado de pronúncia, pausa, ênfase.
- Ideal para criar **narradores automáticos**, **assistentes virtuais**, etc.

---

## 🧪 Recursos Testados

- [x] Conversão de fala em texto com idioma pt-BR
- [x] Detecção automática de idioma
- [x] Exportação de JSON com confiança e timestamps
- [x] Criação de áudios com voz neural

---

## ✅ Conclusão
Speech Studio permite integração simples e poderosa de voz em qualquer aplicação, seja para **acessibilidade, produtividade ou atendimento automático**.

# 🧾 Azure Language Studio – Anotações e Dicas

## 🎯 Objetivo
Utilizar IA para **analisar linguagem natural** de forma automatizada: sentimentos, entidades, tópicos, idioma e muito mais.

---

## 🔹 Recursos Testados

### 1. Análise de Sentimentos
- Detecta polaridade: positivo, neutro, negativo
- Nível: frase e documento
- Retorna pontuações de confiança

### 2. Detecção de Idioma
- Detecta o idioma com base em amostras de texto.
- Útil para sistemas multilíngues.

### 3. Extração de Entidades (NER)
- Identifica nomes, organizações, datas, locais.
- Exemplo:

### 4. Classificação de Texto
- Pode usar categorias predefinidas ou modelos personalizados (via Custom Text Classification).

---

## 🛠️ Como Usar

1. Acesse [language.cognitive.azure.com](https://language.cognitive.azure.com)
2. Escolha um recurso (ex: Análise de Sentimentos)
3. Insira um texto de teste
4. Visualize o JSON de resposta
5. Exporte para reuso

---

## 💡 Dicas Práticas

- Combine **Speech-to-Text + Language Studio** para processar áudios de forma completa.
- Use o JSON para integração com **chatbots, dashboards ou bancos de dados**.
- Crie modelos personalizados se os modelos genéricos não forem suficientes.

---

## 📦 Exemplo de JSON de resposta

```json
{
"sentiment": "positive",
"confidenceScores": {
  "positive": 0.92,
  "neutral": 0.07,
  "negative": 0.01
}
}

---

### ✅ Próximo passo

Você pode criar os arquivos com:

```bash
mkdir -p speech-studio language-studio
touch speech-studio/anotacoes-speech.md
touch language-studio/anotacoes-language.md


