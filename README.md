# App de Finanças Pessoais do Felipe P. B. com Vibe Coding: FelInvestimentos

## 📝 PRD Refinado no Copilot Web

```markdown
📘 PRD – Aplicativo de Organização Financeira com Conversa Natural
1. Visão Geral
O aplicativo será uma solução de organização financeira pessoal baseada em conversas naturais, permitindo que os usuários controlem seus gastos, metas e investimentos sem burocracia.
O diferencial é a experiência conversacional fluida, com um agente financeiro virtual que interpreta linguagem natural e oferece recomendações personalizadas.

2. Problema a Resolver
- Complexidade dos apps atuais: exigem entradas manuais, planilhas e categorias rígidas.
- Baixa adesão: muitos usuários abandonam o controle por falta de praticidade.
- Pouca personalização: recomendações genéricas que não se adaptam ao perfil do usuário.
Solução proposta: um app simples, acessível e inclusivo, que entende frases cotidianas e transforma em registros financeiros automáticos, com dicas personalizadas.

3. Público-Alvo
- Pessoas iniciantes no controle financeiro.
- Usuários que buscam praticidade e acessibilidade.
- Pessoas com baixa familiaridade digital ou que se frustraram com apps tradicionais.

4. Funcionalidades-Chave
- Tela de Início
- Mensagem sobre a importância das finanças.
- Criação de conta com email e senha.
- Registro de Gastos via Chat
- Exemplo: “gastei R$ 30 no mercado”.
- Agente responde de forma acolhedora e educativa.
- Registro automático em categorias.
- Classificação Automática de Transações
- Categorias como alimentação, transporte, lazer.
- Aba “Estatísticas de Consumo” com gráficos e porcentagens.
- Metas Financeiras
- Usuário define metas (ex.: economizar R$ 500 até o fim do mês).
- Agente pode sugerir metas com base nos hábitos.
- Dicas Personalizadas
- Recomendações de economia adaptadas ao perfil.
- Perguntas adicionais para entender melhor o usuário.
- Aba de Investimentos
- Registro de investimentos e rendimentos.
- Gráfico de desempenho a longo prazo.
- Aba de Transações
- Lista de transações correntes, imediatas e agendadas.
- Criação de novas transações via chat ou manualmente.

5. Princípios de Design Universal
- Interface clara e legível.
- Navegação simples e sem sobrecarga.
- Compatibilidade com leitores de tela e comandos por voz.
- Feedback visual e auditivo para confirmar ações.
- Linguagem acessível e amigável.

6. Recursos Técnicos Necessários
- NLP (Processamento de Linguagem Natural) para interpretar frases.
- Motor de Categorização Automática para classificar gastos.
- Motor de Recomendações para dicas personalizadas.
- Banco de Dados Seguro com criptografia.
- Interface Conversacional com suporte a texto e voz.

7. Estratégia de Validação Inicial
- Teste com grupo piloto de usuários iniciantes.
- Feedback rápido via chat após interações.
- Métricas de sucesso:
- Número de transações registradas.
- Metas criadas e acompanhadas.
- Engajamento com dicas do agente.

8. Entregável da IA
- Plano de MVP com telas principais (chat, metas, relatórios).
- Recursos técnicos detalhados.
- Estratégia de validação com usuários reais.
- Linguagem acessível e educativa.
- Aplicação dos princípios de Design Universal desde o protótipo.
```

---

## 💬 Interações com o Lovable

>
```markdown
Crie um app de Finanças com base nesse PRD:: {PRD}
```
>
```markdown
Implementar as seguintes funções no aplicativo:

1. Função de troca de idioma (PT ↔ EN):
   - Criar um botão ou comando no menu de configurações que permita alternar entre português e inglês.
   - Garantir que todos os textos sejam traduzidos corretamente, evitando que partes fiquem em inglês quando o idioma selecionado for português.

2. Ajuste do texto inicial do assistente:
   - Substituir o texto atual:
     "Olá! 👋 Sou seu assistente financeiro. Me conte sobre seus gastos, como: 'gastei R$30 no mercado' ou pergunte sobre suas finanças!"
   - Pelo novo texto:
     "Olá! 👋 Sou seu assistente financeiro. Me conte sobre seus gastos, como: 'gastei R$90 na padaria' ou pergunte sobre suas finanças!"

3. Funções adicionais no chat:
   - Permitir que o usuário crie metas diretamente via conversa (ex.: "Quero economizar R$ 500 até o fim do mês").
   - Adicionar dinheiro às metas já criadas (ex.: "Colocar R$ 100 na meta de viagem").
   - Registrar investimentos via chat (ex.: "Adicione R$ 200 em ações da empresa X").
   - Calcular e mostrar o desempenho dos investimentos ao longo do tempo, exibindo gráficos simples e acessíveis.

4. Requisitos de acessibilidade:
   - Garantir que essas funções estejam disponíveis tanto em texto quanto em comandos de voz.
   - Manter linguagem clara e acessível em todas as respostas do agente financeiro.
```
>
```markdown
Implementar as seguintes funções e ajustes no aplicativo:

1. Histórico do chat:
   - Salvar todas as conversas do usuário com o assistente financeiro.
   - Permitir que o usuário acesse e consulte o histórico dentro do app.

2. Metas e investimentos como transações:
   - Quando o usuário adicionar uma meta ou um investimento, isso deve ser registrado como gasto.
   - Essa regra vale tanto para entradas feitas manualmente quanto via chat.

3. Modificação de valores de investimento:
   - Permitir que o usuário altere o valor atual do investimento em comparação ao valor inicial.
   - O rendimento deve ser calculado automaticamente com base nessa diferença.
   - O chat também deve permitir essa modificação via comandos de linguagem natural.

4. Aba de estatísticas:
   - Ao clicar em "gastos" ou "receitas", mostrar separadamente os pagamentos correntes e os únicos.
   - Adaptar os rótulos “invested” e “current” do gráfico de estatísticas para o idioma escolhido (PT/EN).

5. Aba de metas:
   - Adaptar todos os textos e mensagens da aba de metas ao idioma selecionado (PT/EN).
   - Em especial, adaptar a frase:
     "No goals yet. Create your first one!"
     → para português quando o idioma selecionado for PT.
   - Permitir modificar o quanto já foi colocado em uma meta.
   - A diferença entre o valor antigo e o novo deve ser registrada como transação.
   - Permitir modificar a data da meta tanto manualmente quanto via chat.

6. Chat de voz:
   - Corrigir a funcionalidade do chat de voz, que atualmente não funciona.
   - Garantir que o usuário possa interagir com o assistente usando comandos de voz de forma fluida.

7. Requisitos de acessibilidade:
   - Todas as funções devem estar disponíveis tanto em texto quanto em voz.
   - Manter linguagem clara e adaptada ao idioma selecionado.
```
>
```markdown
Implementar as seguintes funções e ajustes no aplicativo:

1. Chat de voz:
   - Alterar o botão de ativação do microfone para funcionar com clique único:
     - Ícone verde de microfone: microfone ligado.
     - Ícone vermelho de microfone: microfone desligado.
   - O usuário não deve precisar manter o botão pressionado para falar.

2. Exclusão de metas e investimentos:
   - Quando uma meta ou investimento for excluído (manual ou via chat), o valor já colocado na meta ou o valor atual do investimento deve ser convertido em receita.
   - Essa receita deve aparecer nas estatísticas e transações.

3. Pagamentos recorrentes (receitas e gastos fixos):
   - Permitir que os clientes criem pagamentos recorrentes manualmente ou via chat.
   - O usuário deve informar a data em que o pagamento entra na conta.
   - O aplicativo deve considerar a data atual e avaliar se o pagamento já entrou ou não.
   - O cliente pode clicar em um pagamento recorrente e:
     a) Cancelar uma quantidade X de parcelas → remove da receita total o valor correspondente às X parcelas.
     b) Excluir o pagamento recorrente inteiro.
     c) Definir opcionalmente uma data de término → após essa data o pagamento é excluído, mas os valores recebidos até então permanecem registrados.

4. Aba de juros:
   - Adicionar uma aba dedicada para calcular juros.
   - Permitir que o usuário insira valores, taxas e períodos para simulação de rendimento.

5. Estatísticas com moedas estrangeiras:
   - Criar uma aba separada para outras moedas.
   - Se não houver moedas estrangeiras registradas, mostrar mensagem: “Não há outras moedas”.
   - Se houver, mostrar a quantidade de cada moeda (receitas e gastos), incluindo pagamentos recorrentes.
   - Se o usuário tiver 0 de uma moeda, ela deve deixar de aparecer.
   - Permitir que o usuário escolha sua moeda principal na aba de estatísticas.

6. Requisitos de acessibilidade:
   - Todas as funções devem estar disponíveis tanto em texto quanto em voz.
   - Manter linguagem clara e adaptada ao idioma selecionado (PT/EN).
```
>
```markdown
Quero fazer alguns ajustes importantes no site que criei com você. Por favor, siga as instruções abaixo com atenção:
🔄 Troca de moeda principal
- Adicione uma opção para o usuário trocar a moeda principal do site.
- Essa opção deve ficar posicionada acima da opção de mudar o idioma.
- O usuário deve poder digitar manualmente a moeda desejada (ex: USD, BRL, EUR etc).
- A troca de moeda também deve estar disponível diretamente pelo chat.
- Corrija a divisão incorreta das moedas: atualmente “US” e “USD” estão separadas, mas representam a mesma moeda. Unifique corretamente para evitar duplicidade.

💳 Pagamentos recorrentes
- Corrija o sistema de pagamentos recorrentes.
- Reduza ao mínimo possível as informações obrigatórias para criar uma assinatura (apenas o estritamente necessário para funcionamento legal e técnico).
- Revise completamente o código responsável pelos pagamentos recorrentes para garantir que:
- Não haja bugs.
- Não ocorram crashes.
- Não existam conflitos de estado.
- O fluxo de assinatura, renovação e cancelamento funcione corretamente.
- Garanta que o sistema trate corretamente falhas de pagamento, tentativas automáticas de cobrança e cancelamentos.

🛠️ Revisão geral
- Revise a lógica relacionada a moedas e pagamentos para garantir consistência.
- Certifique-se de que todas as alterações sejam aplicadas sem quebrar outras funcionalidades do site.
- Caso seja necessário refatorar partes do código para melhorar estabilidade e organização, faça isso.
```
> 
```markdown
🔄 Troca de moeda
- O campo onde o usuário digita a moeda principal está quebrado. Corrija para que funcione corretamente.
- Quando a moeda é trocada pelo chat, a mudança deve aparecer iimediatamente no site (está apenas aparecendo ao recarregar o site).
- Garanta que a troca funcione de forma consistente em todas as partes do site.

💹 2️⃣ Aba de investimentos para outras moedas
- Adicione uma aba ou seção de investimentos para outras moedas.
- O usuário deve poder selecionar qualquer moeda disponível e visualizar os dados de investimentos correspondentes a essa moeda.
- Certifique-se de que os dados sejam atualizados corretamente ao mudar a moeda.

💳 3️⃣ Pagamentos recorrentes
- Ajuste o sistema de pagamentos recorrentes para permitir períodos além de mensal (ex: semanal, trimestral, anual), tal que o usuário digita o período e a primeira data de recebimento ou pagamento.
- Revise o fluxo de criação, renovação e cancelamento de assinaturas para garantir que funcione em todos os períodos sem bugs ou crashes.
- Mantenha apenas as informações mínimas necessárias para criar a assinatura, sem comprometer o funcionamento.

🛠️ 4️⃣ Revisão geral
- Certifique-se de que todas essas alterações não quebrem outras funcionalidades do site.
- Garanta que o código fique limpo, organizado e funcional.
```

---

## 🎯 Resultado Final

Acesse o protótipo funcional no Lovable:  
**https://appfinancascaixadiofelipe.lovable.app**

<img width="1920" height="945" alt="image" src="https://github.com/user-attachments/assets/88ef611d-970e-4377-918a-918714311218" />

---

## 🔍 Funcionalidades do App de Organização Financeira

### 1. Dashboard Financeiro
- Exibe um panorama claro das finanças pessoais:
  - **Receitas**: Total de ganhos registrados
  - **Despesas**: Total de gastos
  - **Saldo**: Diferença entre receitas e despesas
- Interface simples e direta para facilitar a compreensão

### 2. Assistente Financeiro
- Personagem conversacional que interage com o usuário
- Incentiva a conexão de contas e cartões para uma visão completa das finanças
- Oferece suporte emocional e motivacional

### 3. Registro de Transações via Chat
- Campo de entrada para o usuário digitar mensagens em linguagem natural
- Permite registrar gastos e interagir com o assistente de forma fluida

### 4. Metas Financeiras
- Área dedicada à criação e acompanhamento de objetivos financeiros
- Sugestão proativa para o usuário definir metas
- Botão de ação para adicionar novas metas

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
O refinamento do PRD previamente feito no Copilot ajudou muito, pois os créditos do Lovable acabaram em apenas 3 interações.

### O que não funcionou como o esperado?  
Esperava poder interagir mais vezes gratuitamente com o Lovable, mas as interações feitas já foram de grande valia para aprender mais sobre Vibe Coding.

### O que aprendi sobre conversar com IAs?  
Aprendi que é basicamente igual a conversar com uma pessoa: quanto mais detalhes e clareza você dá, melhor é a interação.
