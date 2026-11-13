Análise de Tarefas
HTA — Iniciar o treino do dia sugerido pelo professor
Funcionalidade: permitir que o idoso identifique rapidamente seu treino diário e inicie a execução guiada dos exercícios.
Estrutura Hierárquica:
0. Iniciar treino (Plano: 1>2>3)
    1. Abrir interface de treinos (Plano: 1/2)
        1.1 Acessar pela aba 'Início' (card em destaque)
        1.2 Acessar pela aba 'Meus treinos' no menu lateral
    2. Identificar o treino do dia (Plano: 1+2)
        2.1 Ler o nome do treino (ex: Força e equilíbrio)
        2.2 Conferir a lista rápida de exercícios
    3. Começar a execução (Plano: 1)
        3.1 Clicar no botão 'Iniciar meu treino'
Planos de execução (HTA 1):
- Plano 0 (1>2>3): acessar a área de treinos, depois identificar o treino correto, depois começar a execução — nessa ordem.
- Plano 1 (1/2): o usuário escolhe um dos atalhos — clicar no card direto na Home ou navegar pelo menu lateral — nunca os dois.
- Plano 2 (1+2): a leitura do nome do treino e a conferência dos exercícios podem ocorrer simultaneamente ou em qualquer ordem.
- Plano 3 (1): apenas executar o clique final de inicialização.
HTA — Confirmar presença em uma aula em grupo
Funcionalidade: permitir que o usuário verifique os horários das aulas coletivas na academia e reserve sua vaga de forma clara.
Estrutura Hierárquica:
0. Confirmar presença na aula (Plano: 1>2>3)
    1. Acessar a agenda (Plano: 1)
        1.1 Tocar no ícone 'Agenda' no menu inferior
    2. Localizar a aula desejada (Plano: 1, depois repetir 2 para analisar outras aulas se necessário)
        2.1 Ler o card da próxima aula disponível
        2.2 Rolar a tela para ver horários posteriores
    3. Confirmar participação (Plano: 1>2)
        3.1 Tocar no botão 'Participar'
        3.2 Verificar o feedback visual de 'Confirmada'
Planos de execução (HTA 2):
- Plano 0 (1>2>3): acessar a agenda, depois localizar a aula, depois confirmar presença — nessa ordem.
- Plano 1 (1): operação única de navegação.
- Plano 2 (1, depois repetir 2...): o usuário lê o primeiro card; se não for o horário desejado, repete a rolagem (loop) até achar a aula certa.
- Plano 3 (1>2): primeiro aperta o botão, depois confere visualmente se o status mudou.
GOMS — Solicitar ajuda rápida da recepção
Funcionalidade: permitir que o usuário (especialmente idosos) faça uma chamada de emergência/dúvida de forma rápida sem se perder no aplicativo.
GOAL 0: ligar para a recepção da academia

  GOAL 1: chegar até a área de contato
  
    METHOD 1.A: usar o botão de emergência global
    (SEL. RULE: o usuário está nas abas Início, Treinos, Agenda ou Perfil, onde o menu lateral está visível)
      OP. 1.A.1: localizar visualmente o card 'Precisa de ajuda?' no canto inferior esquerdo
      OP. 1.A.2: tocar no botão 'Ligar'

    METHOD 1.B: voltar da tela de execução
    (SEL. RULE: o usuário está no meio de um exercício na tela cheia e sente desconforto)
      OP. 1.B.1: tocar no ícone de interrogação [?] no rodapé
      
  GOAL 2: confirmar a chamada no celular
    METHOD 2.A: iniciar discagem
      OP. 2.A.1: aguardar o sistema operacional abrir a tela do telefone
      OP. 2.A.2: tocar no botão verde de ligar do próprio celular
GOMS — Visualizar evolução semanal e metas (Meu Progresso)
Funcionalidade: permitir que o familiar responsável ou o próprio idoso cheque rapidamente a assiduidade e o tempo de atividade cumprido no mês.
GOAL 0: visualizar se o idoso cumpriu a meta de exercícios da semana

  GOAL 1: acessar os dados de frequência

    METHOD 1.A: verificar a visão rápida na Home
    (SEL. RULE: o usuário quer apenas saber se o treino de hoje ou de ontem foi feito, sem detalhes profundos)
      OP. 1.A.1: tocar na aba 'Início'
      OP. 1.A.2: localizar visualmente o bloco 'Visão da Semana'
      OP. 1.A.3: conferir os selos de check nos dias da semana

    METHOD 1.B: acessar o painel completo de Progresso
    (SEL. RULE: o responsável familiar precisa ver o tempo total e a barra de progressão mensal)
      OP. 1.B.1: tocar na aba 'Meu progresso' no menu lateral
      OP. 1.B.2: aguardar o carregamento do painel central
      
  GOAL 2: interpretar as estatísticas na tela de Progresso
    METHOD 2.A: ler métricas ativas
      OP. 2.A.1: ler o número de 'Treinos realizados'
      OP. 2.A.2: verificar a barra de 'Meta do Mês'
