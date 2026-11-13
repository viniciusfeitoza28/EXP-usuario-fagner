Requisitos de UX e Metas de Usabilidade

Ciclo de vida de usabilidade do Projeto Viva Bem

Este documento reúne os requisitos de experiência do usuário do Viva Bem ("Saúde em movimento"), aplicação web para acompanhamento de treinos, aulas e progresso de saúde, voltada a adultos e idosos e aos seus responsáveis. Ele corresponde à etapa de análise de requisitos do ciclo de vida de usabilidade: características da plataforma, princípios gerais de projeto e metas de usabilidade.

1. Características da Plataforma
Característica	Descrição
Descrição do Software	Aplicação web responsiva, com protótipo de alta fidelidade criado no Figma e publicado no Figma Sites, e implementação em React. A navegação é organizada em seis seções: Início, Meus treinos, Agenda, Meu progresso, Meu perfil e Meu responsável. Os dados exibidos na versão atual são fictícios e servem para demonstração.
Descrição do Hardware	O uso principal é em smartphones, com tela sensível ao toque, e o uso secundário em tablets e computadores. Basta um navegador atual e conexão com a internet. Não é necessário nenhum hardware especial.
Lista de capacidades da plataforma	Responsividade: o layout se adapta a telas pequenas e grandes, com barra de navegação inferior no celular e menu superior no computador. Interação por toque: botões grandes e espaçados facilitam o uso por pessoas com menor precisão motora. Ampliação do texto: o botão "Aa" aumenta o tamanho da fonte em qualquer tela. Chamada telefônica: o botão "Ligar" abre o discador do aparelho com o número da recepção. Acompanhamento visual: o calendário da semana, as barras de progresso e as marcações de treino concluído mostram a evolução de forma imediata. Acesso sem instalação: o uso é direto pelo navegador, sem baixar aplicativo.
Lista de restrições da plataforma	Dependência de internet: sem conexão, o conteúdo não carrega. Sem cadastro e sem dados reais: a versão atual não tem login nem banco de dados, então o progresso não é salvo entre acessos. Sem notificações: não há lembretes automáticos de treino ou de aula. Chamada telefônica limitada: em computadores sem telefonia, o botão de ligar pode não funcionar. Telas pequenas: o espaço reduzido obriga a mostrar pouca informação por vez. Experiência do público-alvo com tecnologia: parte dos usuários tem pouca familiaridade com aplicativos, o que limita o uso de gestos e recursos escondidos.
2. Princípios Gerais do Projeto
Nome	Descrição	Link
LGPD (Lei 13.709/2018)	Regula o tratamento de dados pessoais. Como o aplicativo trata nome, idade, telefone, dados de saúde e dados do responsável, é preciso coletar apenas o necessário, informar a finalidade e proteger essas informações.	Planalto
Lei 10.098/2000	Estabelece normas gerais de acessibilidade para pessoas com deficiência ou mobilidade reduzida, entre elas a eliminação de barreiras na comunicação. Orienta o projeto de uma interface que todos consigam usar.	Planalto
Lei 13.146/2015 (Lei Brasileira de Inclusão)	Garante direitos de acesso à informação e à comunicação, inclusive em sites e aplicativos. Reforça a necessidade de acessibilidade digital no Viva Bem.	Planalto
Lei 10.741/2003 (Estatuto da Pessoa Idosa)	Assegura à pessoa idosa direitos à saúde, ao esporte e à informação adequada. Fundamenta o foco do projeto em atividades físicas leves e em uma comunicação respeitosa e clara.	Planalto
ABNT NBR ISO 9241	Conjunto de normas sobre ergonomia da interação humano-sistema. A parte 210 trata do projeto centrado no ser humano, e a parte 11 define usabilidade por eficácia, eficiência e satisfação, base das metas deste documento.	ISO 9241-210 e ISO 9241-11
WCAG 2.1 (W3C)	Diretrizes internacionais de acessibilidade para conteúdo web, baseadas nos princípios perceptível, operável, compreensível e robusto. Orientam o contraste de cores, o tamanho do texto, o tamanho dos alvos de toque e a navegação por teclado.	W3C
10 heurísticas de Nielsen	Princípios gerais de usabilidade, como visibilidade do estado do sistema, prevenção de erros, reconhecimento em vez de memorização e linguagem do mundo real. Servem de guia de projeto e de base para a avaliação heurística.	Nielsen Norman Group
Descrição do Contexto	O Viva Bem é usado no dia a dia, principalmente no celular, em casa ou no local de treino, antes ou depois das atividades físicas. O público é formado por adultos e idosos, com possível baixa visão, menor precisão motora e pouca experiência com tecnologia, que podem contar com o apoio de um familiar ou cuidador. O contexto exige textos legíveis, poucas escolhas por tela, linguagem simples e botões grandes.	-
3. Metas de Usabilidade

As metas foram definidas a partir das normas e heurísticas acima e distribuídas por peso, de modo que cada tabela some 100%. O peso indica a prioridade da meta para o público do projeto.

Qualitativo
Metas	Porcentagem	Justificativa
Facilidade de aprendizado	25%	A pessoa deve conseguir usar o aplicativo na primeira vez, sem treinamento e sem manual, pois parte do público tem pouca experiência com tecnologia.
Legibilidade e acessibilidade	25%	Texto grande, bom contraste e alvos de toque amplos são necessários para quem tem baixa visão ou menor precisão motora.
Facilidade de uso e eficiência	10%	As tarefas principais (iniciar o treino, ver a agenda, acompanhar a semana) devem exigir poucos toques.
Facilidade de lembrar	10%	Quem usa o aplicativo de vez em quando precisa reencontrar as funções sem reaprender, o que é favorecido por poucas seções e nomes consistentes.
Prevenção e recuperação de erros	15%	Erros de toque não podem causar perda de dados nem confusão. As mensagens devem ser claras e a volta a uma tela anterior deve ser sempre simples.
Satisfação subjetiva	15%	A linguagem positiva e o retorno visual do progresso devem motivar a continuidade, sem gerar pressão ou constrangimento.
Total	100%	
Quantitativo
Metas	Porcentagem	Justificativa
Pelo menos 90% dos participantes iniciam o treino do dia sem ajuda e em até 1 minuto	25%	Iniciar o treino é a tarefa central do produto e mede a facilidade de aprendizado e a eficiência.
Pelo menos 90% dos participantes encontram a próxima aula na agenda em até 30 segundos	20%	Consultar a agenda é uma das tarefas mais frequentes, e a rapidez indica que a informação está bem organizada.
Média de, no máximo, 1 erro por tarefa (por exemplo, toques em locais errados ou voltas desnecessárias)	15%	Poucos erros mostram que os botões e os textos são claros e que o fluxo é previsível.
Pelo menos 80% dos participantes localizam e usam o botão de aumentar o texto na primeira tentativa	15%	A ampliação do texto é um recurso de acessibilidade essencial e precisa ser descoberta sem ajuda.
Pontuação média igual ou superior a 80 na escala SUS (System Usability Scale)	15%	A escala SUS é uma medida padronizada de satisfação, e 80 pontos indica boa usabilidade, acima da média de 68.
Pelo menos 85% dos participantes repetem as tarefas principais, em uma segunda sessão, sem ajuda	10%	Mede a facilidade de lembrar o caminho depois de um intervalo de uso.
Total	100%	

Os valores quantitativos serão verificados no teste de usabilidade com observação do usuário, conforme o planejamento da avaliação.
