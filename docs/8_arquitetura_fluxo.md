Arquitetura de Informação e Fluxos de Usuário
Projeto Viva Bem – Aplicativo de Academia para Idosos
1. Arquitetura de Informação (Sitemap)
A arquitetura de informação do aplicativo Viva Bem foi projetada para ser o mais plana (flat) possível, evitando menus profundos que causam desorientação espacial no público idoso. Todo o conteúdo principal está a um clique de distância a partir da barra de navegação lateral fixa.
Diagrama de Sitemap (Hierarquia de Telas):
•	Global (Visível em todas as telas)
Cabeçalho: Acessibilidade ("Aa Aumentar texto") | Avatar do Perfil
Menu Lateral: Navegação principal
Card Inferior: "Precisa de ajuda? Ligar" (Botão de emergência fixo)
1. Início (Home)
* Card Primário: Seu Próximo Treino (Ação: Iniciar meu treino)
* Visão da Semana: Resumo rápido do ritmo (check-ins)
* Próxima Aula: Card de lembrete com botão de atalho para a Agenda
* Dica para Hoje: Lembretes rápidos de saúde (ex: beber água)
2. Meus Treinos
* Plano atualizado pelo professor (Lista de exercícios)
•   ↳ [Ação] Detalhar exercício (Revelação Progressiva das métricas)
•   ↳ [Ação] Iniciar Treino -> Tela de Execução:
•       - Vídeo/Animação do movimento
•       - Temporizador / Séries
•       - Controles: [Pausar] | [Terminei este exercício]
3. Agenda
* Lista de Aulas em Grupo (Data, Horário, Professor, Vagas)
•   ↳ [Ação] Confirmar Participação / Cancelar
4. Meu Progresso
* Estatísticas: Treinos realizados, Tempo em movimento, Sequência atual
* Meta do mês (Barra de progresso)
* Conquistas recentes (Gamificação leve)
5. Meu Perfil
* Dados Pessoais (Telefone, Contato de Emergência)
* Cuidados de saúde informados (Restrições médicas)
* Configuração do Sistema: Toggle "Texto maior"
6. Meu Responsável
* Código de vínculo (ex: VB-2403-MS)
* Formulário de cadastro do familiar/cuidador de confiança
Justificativa baseada nas Personas e Cenários:
A organização plana com uma barra de navegação sempre visível atende diretamente à dor da Persona Maria (Primária 1), que se frustra quando se perde em menus complexos. Ao colocar o card 'Seu Próximo Treino' logo na tela Início, reduzimos a fricção e o tempo de decisão (GOMS estimado em 2 a 3 segundos). A aba Agenda separada foi estruturada para o Roberto (Primária 2), permitindo que ele foque em marcar suas aulas coletivas sem se misturar com configurações. Já a aba Meu Progresso serve como um hub direto para a Ana (Secundária - Responsável) conferir rapidamente os resultados do pai sem interferir nos exercícios do dia.
2. Fluxos do Usuário (User Flows)
Abaixo estão os 4 fluxos principais de tarefas que balizam a interação dos idosos e responsáveis com o aplicativo, otimizados após os testes de prototipação em papel.
Fluxo 1: Iniciar e Concluir o Treino do Dia (Principal)
•	Funcionalidade e Objetivo: Permitir que o aluno idoso inicie seu treino diário com o menor esforço cognitivo possível, sendo guiado passo a passo até a conclusão.
Fluxograma:
1. [Tela: Início] O usuário abre o app.
2. [Decisão] Quer iniciar o treino sugerido? (Sim).
3. [Ação] Clica no botão central verde 'Iniciar meu treino' (Card Seu Próximo Treino).
4. [Tela: Execução] O sistema exibe o Exercício 1 de N (ex: Aquecimento na esteira).
5. [Ação] Usuário realiza o exercício assistindo ao vídeo/timer.
6. [Decisão] Precisou descansar no meio? -> Clica em [Pausar] -> Retoma depois.
7. [Ação] Clica no botão grande 'Terminei este exercício'.
8. [Repetição] O fluxo se repete para os próximos exercícios até o fim da lista.
9. [Sucesso] Tela de feedback celebrando o término do treino e atualizando a meta.
Atalho / Caminho Alternativo: O usuário pode clicar na aba 'Meus treinos' no menu lateral para revisar toda a lista de exercícios detalhada antes de apertar o botão 'Iniciar treino' no final da página.
Fluxo 2: Confirmar Presença em Aula Coletiva
•	Funcionalidade e Objetivo: Garantir que o idoso (como o Roberto) consiga visualizar as aulas disponíveis e reservar sua vaga rapidamente e sem erros.
Fluxograma:
1. [Tela: Início] O usuário clica no menu lateral 'Agenda'.
2. [Tela: Agenda] O sistema lista os cards das aulas futuras com datas, salas e vagas restantes.
3. [Decisão] Localiza a aula desejada (ex: Alongamento em grupo).
4. [Ação] Clica no botão verde escuro 'Participar'.
5. [Sucesso] O botão muda imediatamente para estado claro com ícone de check: 'Confirmada'. Feedback visual imediato para prevenir toque duplo.
Atalho / Caminho Alternativo: Se a próxima aula estiver próxima, ela aparecerá em um card de atalho 'Próxima Aula' diretamente na tela de Início, com um link rápido 'Ver minha agenda' ou botão de confirmar, poupando a navegação. Para cancelar (Erro/Desistência), o usuário apenas toca novamente no botão 'Confirmada'.
Fluxo 3: Acompanhamento de Frequência e Metas
•	Funcionalidade e Objetivo: Permitir que o idoso acompanhe suas conquistas ou que o familiar responsável visualize se a rotina de exercícios está sendo mantida.
Fluxograma:
1. [Tela: Início] O responsável ou aluno acessa o aplicativo.
2. [Ação] Clica no menu lateral 'Meu progresso'.
3. [Tela: Meu progresso] O sistema carrega o painel central.
4. [Decisão visual] O usuário verifica os cards de 'Treinos realizados', 'Tempo em movimento' e a barra de 'Meta do Mês'.
5. [Sucesso] Tarefa concluída passivamente pela leitura dos dados (Tempo de GOMS: ~2 segundos).
Atalho / Caminho Alternativo: O idoso não precisa acessar essa tela todos os dias, pois a Tela Início já possui o micro-componente 'Visão da Semana: Seu ritmo está ótimo', que exibe checks rápidos dos dias em que ele já treinou, funcionando como um atalho visual de status.
Fluxo 4: Solicitar Ajuda Rápida (Emergência/Dúvida)
•	Funcionalidade e Objetivo: Garantir segurança de uso. Idosos podem sentir dor ou ter dúvidas sobre a execução do equipamento e precisam de contato imediato com o professor ou recepção.
Fluxograma:
1. [Qualquer Tela do App] O usuário se sente inseguro ou tem dúvidas.
2. [Ação] O usuário localiza o bloco permanente no canto inferior esquerdo 'Precisa de ajuda? Fale com a recepção'.
3. [Ação] Clica no texto 'Ligar: 4002-0220'.
4. [Sucesso] O sistema operacional do celular intercepta a ação e abre o teclado de discagem rápida já com o número preenchido.
Atalho / Caminho Alternativo: Durante os testes de protótipo em papel, foi solicitada a inclusão de um botão discreto de interrogação [?] no rodapé da própria Tela de Execução para não obrigar o idoso a cancelar o exercício inteiro só para tirar uma dúvida rápida (oportunidade de melhoria mapeada).
