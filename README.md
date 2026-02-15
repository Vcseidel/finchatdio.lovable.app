# 💸 App de Finanças Pessoais do Victor com Vibe Coding

Este projeto foi desenvolvido como um Desafio de Projeto da DIO de Vibe Coding utilizando o Lovable e o Gemini da google. A proposta é criar um aplicativo de organização financeira pessoal baseado em interações em linguagem natural.

---

## 📝 PRD Refinado no Gemini

```markdown
# PRD - FinChat: Assistente Financeiro e Investimentos

## 1. Visao Geral
O FinChat e um aplicativo de gestao financeira pessoal e educacao em investimentos baseado em uma interface de chat (Chat-First). O objetivo e permitir que usuarios iniciantes organizem suas financas e aprendam sobre investimentos atraves de linguagem natural, eliminando a barreira de planilhas complexas.

## 2. Publico-Alvo
Pessoas que desejam iniciar o controle financeiro e entrar no mundo dos investimentos, mas sentem-se intimidadas por termos tecnicos ou interfaces saturadas de informacao.

## 3. Principios de Design Universal
- Simplicidade: Interface limpa com foco na conversa.
- Acessibilidade: Navegacao via teclado, suporte a leitores de tela e alto contraste.
- Legibilidade: Fontes grandes e espacamento adequado.
- Feedback: Confirmacoes claras para cada acao realizada pelo usuario.

## 4. Funcionalidades de Conversa (NLP)
- Registro de Gastos: O usuario digita frases como "Gastei 50 reais em almoco" e o sistema categoriza como Alimentacao.
- Registro de Investimentos: O usuario digita "Investi 200 reais em Tesouro Selic" e o sistema move o valor para a carteira de ativos.
- Consulta de Saldo: O usuario pergunta "Quanto eu tenho?" e o sistema retorna o saldo em conta e o total investido.

## 5. Modulos de Investimento (Educativo e Gestao)
O sistema deve gerenciar e explicar as seguintes categorias de ativos:

- Renda Fixa: Emprestimos para bancos ou governo (Ex: CDB, Tesouro Direto). Foco em seguranca.
- Renda Variavel: Acoes de empresas. Foco em crescimento de longo prazo, com maior risco.
- Fundos Imobiliarios (FIIs): Investimento em imoveis que gera renda mensal (dividendos).
- ETFs (Fundos de Indice): Cestas de ativos que replicam indices (Ex: BOVA11, IVVB11).
- Reserva de Valor: Ativos para protecao contra inflacao ou crises (Ex: Ouro, Bitcoin).

## 6. Componentes de Interface (UI)
- Janela de Chat: Area principal de interacao.
- Dashboard de Patrimonio: Grafico simples mostrando a divisao entre Saldo Disponivel e Total Investido.
- Glossario de Ativos: Cards informativos que explicam o conceito de cada tipo de investimento ao clicar.

## 7. Estrutura de Dados Sugerida
O estado da aplicacao deve seguir esta estrutura base:

{
  "conta": {
    "saldo_disponivel": 0.0,
    "total_investido": 0.0
  },
  "transacoes": [
    { "id": "uuid", "tipo": "despesa", "valor": 0.0, "categoria": "string", "data": "iso-date" }
  ],
  "investimentos": [
    { "id": "uuid", "classe": "renda_fixa", "nome": "string", "valor": 0.0 }
  ]
}

## 8. Requisitos Tecnicos para o MVP
- Framework: React com Tailwind CSS.
- Biblioteca de Componentes: Shadcn/UI (Acessivel).
- Graficos: Recharts.
- Persistencia: LocalStorage para armazenamento local no navegador.
- Logica de Processamento: Analise de strings via Regex para identificar valores, categorias e tipos de ativos.

## 9. Criterios de Aceite
- O usuario deve conseguir registrar uma despesa em menos de 5 segundos via chat.
- O sistema deve diferenciar visualmente o que e gasto do que e investimento.
- O Glossario deve exibir definicoes didaticas para todas as 5 categorias de investimento citadas.
- A interface deve ser totalmente responsiva para dispositivos moveis.

##10. Pontos de atenção:

Gere o código inicial deste projeto usando React e Tailwind. Comece criando a tela de Chat e a lógica de processamento de texto.

Para este MVP, NÃO conecte em APIs de bolsa de valores externas. Trate os investimentos como valores estáticos inseridos pelo usuário. O foco é a interface educativa e a categorização via chat, não a cotação em tempo real.
```

---

## 💬 Interações com o Lovable

> Olá Lovable, crie uma aplicação de finanças pessoais seguindo o PRD(Product Requirement Document) a seguir: {PRD}

> Gostei da aplicação gostaria de propor algumas alterações, poderia incluir no dashboard um campo para despesas, além disso, gostaria de incluir um modulo de rastreio de investimentos. Além disso colocar os conceitos de investimento para serem respondidos no chat



---

## 🎯 Resultado Final

Acesse o protótipo funcional no Lovable:  https://finchatdio.lovable.app/


<img width="698" height="866" alt="image" src="https://github.com/user-attachments/assets/6d71b8d6-7b5a-44bf-9dd0-a21a3233c5eb" />


---

## 🔍 Funcionalidades do App de Organização Financeira

### 1. Dashboard Financeiro
- Exibe um panorama claro das finanças pessoais:
  - **Receitas**: Total de ganhos registrados
  - **Despesas**: Total de gastos
  - **Investimento**: total investido
  - **Patrimonio**: Diferença entre receitas e despesas
- Interface simples e direta para facilitar a compreensão

### 2. Assistente Financeiro
- Interage com o usuário para inlusão de valores

### 3. Registro de Transações via Chat
- Campo de entrada para o usuário digitar mensagens em linguagem natural
- Permite registrar gastos e interagir com o assistente de forma fluida

### 4. Metas Financeiras
- Área dedicada à investimentos
- Glossario de investimentos para educação geral na hora de investir
- demarcação de despesas gerais

### 5. Relatórios Personalizados
- Visualizações simples e adaptadas ao estilo do usuário
- Acompanhamento de metas e progresso financeiro

### 6. Design Universal
- Interface acessível e inclusiva:
  - Linguagem simples
  - Navegação clara
  - Compatibilidade com leitores de tela e comandos por voz
  - Feedbacks visuais e auditivos para facilitar o uso

---

## 🧠 Reflexão

### O que funcionou bem?  
O refinamento via Gemini Pro, os pontos de atenção demarcados 

### O que não funcionou como o esperado?  
Não diferenciei os modulos de despesa

### O que aprendi sobre conversar com IAs?  
Detalhes devem ser claros e bem expostos
