# Painel BI Faturamento - v1 modular

Estrutura:
- `index.html`
- `css/faturamento.css`
- `js/app.js`

Objetivo:
- Deixar o painel mais leve e mais fácil de manter.
- Preservar os cálculos e a integração atual com Supabase.

Teste recomendado:
1. Abrir `index.html` localmente.
2. Pressionar F12 → Console.
3. Verificar se não há erro de CSS/JS.
4. Testar Dashboard, Diário, Gráficos, Anual e Config.


## v4 - Config preservado
- Mantida a estrutura original do menu e da aba Config.
- Removido bloqueio efetivo do menu pai.
- Receitas adicionais são inseridas via JavaScript dentro da aba Config.
- Bruto gerencial = bruto operacional + receitas adicionais.
- Líquido = bruto gerencial - setor.


## v5 - Sem bloqueio do Config
- Força todos os botões do menu como visíveis.
- Remove bloqueio visual do botão Config.
- Mantém receitas adicionais e acesso direto.


## v6 - Descontos gerenciais
- Adicionado campo "Descontos gerenciais do mês" no Config.
- Cálculo líquido passa a considerar:
  bruto operacional + receitas adicionais - setor - descontos.
- Descontos ficam salvos localmente no navegador.


## v7 - Ajustes Gerenciais Compacto
- Receita adicional e desconto exibidos lado a lado.
- Resumo de impacto líquido abaixo.
- Mantém toda a lógica da v6.
