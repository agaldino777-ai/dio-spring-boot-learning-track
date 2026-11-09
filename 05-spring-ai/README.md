# 🚀 API Inteligente de Orçamento com Spring AI (Desafio DIO)

## 📌 Sobre o Projeto
Esta aplicação é uma API REST desenvolvida em **Spring Boot** integrada com **Spring AI**. O sistema recebe comandos de voz ou texto sobre transações financeiras, processa as intenções com inteligência artificial, executa funções da aplicação (*Tool Calling*) e retorna respostas estruturadas em texto e áudio MP3.

---

## 🛠️ Tecnologias Utilizadas
- **Java 17+** & **Spring Boot**
- **Spring AI** (ChatClient, Speech-to-Text e Text-to-Speech)
- **OpenAI API**
- **Gradle**
- **Docker Compose**

---

## 🔄 Fluxo Principal da API
1. **Envio de Áudio:** O utilizador envia um ficheiro de áudio com o comando financeiro.
2. **Transcrição (STT):** O modelo `TranscriptionModel` converte o áudio em texto.
3. **Processamento com IA:** O `ChatClient` interpreta a intenção da mensagem.
4. **Execução de Função (Tool Calling):** A IA chama os casos de uso da aplicação mapeados com `@Tool`.
5. **Resposta em Voz (TTS):** O `TextToSpeechModel` gera uma resposta final em ficheiro MP3.

---

## ✨ Melhoria Implementada
- **Documentação Completa do Fluxo e Execução:** Estruturação e detalhamento do guia de utilização no `README.md`, facilitando a execução do projeto, o entendimento da arquitetura e o teste dos endpoints.

---

## 🚀 Como Executar a Aplicação

1. Defina a sua chave da OpenAI no terminal:
   ```bash
   export OPENAI_API_KEY="sua_chave_aqui"
