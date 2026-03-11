# Jornadas de Usuário — MVP StockPay (Fase 1)

> Escopo restrito à Fase 1 — Validação do Problema e MVP Operacional (0–4 meses).

---

• Persona: Carlos — Dono de Pequeno Varejo / Decisor Principal
  • Objetivo da jornada: Acessar o sistema com segurança, cadastrar produtos e acompanhar as vendas pelo dashboard para ter controle total da operação.
  • Jornadas a construir (MVP):

    • 1. Acessar o sistema com login seguro
      • Jobs funcionais: "Entrar no sistema com meu e-mail e senha para ter acesso exclusivo ao painel do dono."
      • Jobs emocionais: "Sentir que meu negócio está protegido e que nenhum funcionário acessa o que não deveria."
      • Touchpoints: Tela de Login → Inserir e-mail + senha forte → Validação de credenciais → Dashboard Principal (role Owner).

    • 2. Cadastrar novo produto no sistema
      • Jobs funcionais: "Registrar nome, código e estoque inicial de um produto para que ele fique disponível no PDV e no controle de estoque."
      • Jobs emocionais: "Sentir controle total do catálogo sem depender de planilha ou caderno."
      • Touchpoints: Dashboard Principal → Menu "Produtos" → Tela de Lista de Produtos → Botão "Novo Produto" → Formulário de Cadastro (nome, código, quantidade) → Confirmar → Feedback de sucesso → Lista de Produtos atualizada.

    • 3. Editar e ajustar estoque manualmente
      • Jobs funcionais: "Corrigir a quantidade de um produto após identificar divergência entre o físico e o digital."
      • Jobs emocionais: "Sentir tranquilidade ao saber que consigo corrigir erros antes que virem prejuízo."
      • Touchpoints: Dashboard Principal → Menu "Estoque" → Tela de Gerenciamento de Estoque → Buscar produto → Editar quantidade → Registrar motivo do ajuste → Salvar → Log de auditoria gerado → Estoque atualizado.

    • 4. Acompanhar vendas pelo dashboard
      • Jobs funcionais: "Consultar o resumo de vendas do mês e o lucro estimado para saber se o negócio está indo bem."
      • Jobs emocionais: "Sentir clareza financeira ao ver os números da loja em um painel simples, sem precisar de contador."
      • Touchpoints: Dashboard Principal → Painel de Resumo Mensal → Visualizar total de vendas, formas de pagamento e lucro estimado → Filtro por período.

---

• Persona: Juliana — Caixa / Operadora de PDV
  • Objetivo da jornada: Autenticar-se no sistema com perfil individual e realizar vendas de forma ágil e sem erros pelo PDV.
  • Jornadas a construir (MVP):

    • 1. Acessar o sistema com perfil de Caixa
      • Jobs funcionais: "Fazer login com meu usuário para que minhas vendas fiquem registradas separadas dos outros operadores."
      • Jobs emocionais: "Sentir segurança de que tudo que faço fica registrado no meu nome, sem risco de erro de outro caixa cair sobre mim."
      • Touchpoints: Tela de Login → Inserir e-mail + senha → Validação → Tela de PDV (perfil Cashier) → Nome do operador ativo exibido no topo → Acesso restrito às funções do perfil Caixa.

    • 2. Buscar produto e montar carrinho de venda
      • Jobs funcionais: "Pesquisar um produto por nome ou código e adicioná-lo ao carrinho sem precisar navegar por menus."
      • Jobs emocionais: "Sentir agilidade no atendimento mesmo no horário de pico, sem medo de errar o item ou a quantidade."
      • Touchpoints: Tela de PDV → Campo de Pesquisa Rápida (nome ou código) → Resultado com nome e preço → Adicionar ao Carrinho → Carrinho Editável com ajuste de quantidade → Remoção de item se necessário → Subtotal atualizado em tempo real.

    • 3. Finalizar venda e registrar pagamento
      • Jobs funcionais: "Escolher a forma de pagamento, confirmar o valor e fechar a venda sem etapas desnecessárias."
      • Jobs emocionais: "Trabalhar com tranquilidade sabendo que o sistema registra tudo certo e que não vou errar o troco ou esquecer de lançar uma venda."
      • Touchpoints: Carrinho com itens → Botão "Finalizar Venda" → Tela de Pagamento → Selecionar forma: PIX / Dinheiro / Cartão → (se dinheiro) Inserir valor recebido → Cálculo automático do troco → Confirmar pagamento → Venda registrada → Baixa automática no estoque → Tela de PDV zerada para próximo atendimento.


> Escopo restrito à Fase 2 — Confiabilidade Operacional e Gestão de Estoque (4–8 meses)

• Persona: Carlos — Dono de Pequeno Varejo / Decisor Principal
  • Objetivo da jornada: Agendar entregas de remessas de fornecedores, confirmar o recebimento no dia previsto e analisar o desempenho dos produtos pelo dashboard analítico para tomar decisões de reposição com base em dados reais.

  • Jornadas a construir (Fase 2):

    • 1. Acessar o sistema com login seguro
      • Jobs funcionais: "Entrar no sistema com meu e-mail e senha para ter acesso exclusivo ao painel do dono."
      • Jobs emocionais: "Sentir que meu negócio está protegido e que nenhum funcionário acessa o que não deveria."
      • Touchpoints: Tela de Login → Inserir e-mail + senha forte → Validação de credenciais → Dashboard Principal (role Owner).

    • 2. Agendar entrega de remessa de fornecedor
      -  Jobs funcionais: "Cadastrar uma entrega futura informando os produtos esperados, as quantidades e a data prevista, para que o sistema me lembre e registre o recebimento no dia certo."
      -  Jobs emocionais: "Sentir que tenho controle sobre o que está chegando na loja sem depender de anotação em papel ou de memória."
      -  Touchpoints: Dashboard Principal → Menu "Entregas" → Tela de Agendamentos → Botão "Nova Entrega" → Formulário de Agendamento (fornecedor, produtos, quantidades esperadas, data prevista) → Confirmar → Entrega salva e listada no calendário do sistema → No dia agendado: notificação automática exibida ao dono "A entrega de [Fornecedor] está prevista para hoje. O que aconteceu?" → Tela de Confirmação de Entrega com 3 opções:
        ◦ ✅ Chegou completa → Confirmar → Estoque atualizado automaticamente com as quantidades previstas → Entrega registrada no histórico de movimentações.
        ◦ ⚠️ Chegou parcialmente → Campo para inserir a quantidade real recebida por produto → Confirmar → Estoque atualizado com as quantidades informadas → Divergência registrada no histórico → Alerta de pendência gerado.
        ◦ ❌ Não chegou → Confirmar não recebimento → Entrega marcada como pendente → Registro no histórico → Opção de reagendar para nova data.

    • 3. Acessar o dashboard analítico de produtos
      -  Jobs funcionais: "Consultar o relatório de produtos mais vendidos e produtos parados para decidir o que repor, o que promover e o que deixar de comprar."
      -  Jobs emocionais: "Sentir que estou tomando decisões baseadas em dados reais da minha loja, não no chute — e que não vou mais perder dinheiro comprando o que não vende."
      -  Touchpoints: Dashboard Principal → Menu "Relatórios" → Tela de Dashboard Analítico → Visualizar ranking de produtos mais vendidos (por quantidade e faturamento) → Visualizar lista de produtos parados (sem movimentação no período) → Filtro por período (semana / mês) → Leitura dos dados consolidados → Decisão de reposição ou promoção baseada nos relatórios exibidos.


• Persona: Carlos — Dono de Pequeno Varejo / Decisor Principal

  • Objetivo da jornada: Assinar o plano Premium do EstoquePay diretamente pelo sistema, escolhendo entre o plano Mensal ou Anual, para desbloquear funcionalidades avançadas como o agendamento de entregas.

  • Jornadas a construir (Fase 2):

    • 1. Contratar assinatura Premium do EstoquePay
      -  Jobs funcionais: "Escolher um plano de assinatura e pagar diretamente pelo sistema para desbloquear as funcionalidades avançadas sem precisar sair do app ou falar com ninguém."
      -  Jobs emocionais: "Sentir que estou investindo no crescimento da minha loja com segurança, sabendo exatamente o que vou pagar e o que vou ganhar em troca."
      -  Touchpoints: Dashboard Principal → Banner ou bloqueio de funcionalidade Premium (ex: "Agendamento de Entregas — disponível no plano Premium") → Botão "Assinar Agora" → Tela de Planos → Comparativo entre Plano Mensal e Plano Anual (preço, benefícios e economia) → Seleção do plano desejado → Tela de Pagamento via gateway (ex: AbacatePay) → Escolha da forma de pagamento: PIX / Cartão de Crédito → Inserir dados de pagamento → Confirmar pagamento → Processamento pelo gateway → Feedback de assinatura ativada com sucesso → Dashboard atualizado com selo Premium visível → Funcionalidades desbloqueadas liberadas imediatamente → E-mail de confirmação de assinatura enviado ao dono.