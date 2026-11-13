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

<svg xmlns="http://www.w3.org/2000/svg" width="1600" height="1250" viewBox="0 0 1600 1250" font-family="DejaVu Sans Condensed, Arial Narrow, Arial, sans-serif">
<defs><marker id="a" viewBox="0 0 10 10" refX="9" refY="5" markerWidth="8" markerHeight="8" orient="auto-start-reverse"><path d="M0,0 L10,5 L0,10 z" fill="#3b3b3b"/></marker></defs>
<rect width="1600" height="1250" fill="#ffffff"/>
<text x="800.0" y="34" text-anchor="middle" font-size="30" font-weight="700" fill="#1f5a41">Ciclo de vida de usabilidade do Projeto Viva Bem</text>
<text x="800.0" y="58" text-anchor="middle" font-size="16" fill="#4d5b53">Etapa em destaque: Análise de requisitos (requisitos de UX e metas de usabilidade)</text>
<g transform="translate(0,70)">
<rect x="20" y="20" width="1560" height="300" rx="20" fill="none" stroke="#0d47a1" stroke-width="3"/>
<text x="45" y="302" font-size="18" font-weight="700" fill="#0d47a1">ANÁLISE DE REQUISITOS</text>
<rect x="65" y="45" width="330" height="95" rx="10" fill="#1976d2" stroke="#0d47a1" stroke-width="2"/>
<text x="230.0" y="82.1" text-anchor="middle" font-size="21" font-weight="700" fill="#fff">Perfil do usuário</text>
<text x="230.0" y="102.2" text-anchor="middle" font-size="14" font-weight="400" fill="#fff">Adultos e idosos com treinos leves</text>
<text x="230.0" y="120.4" text-anchor="middle" font-size="14" font-weight="400" fill="#fff">e seus responsáveis</text>
<path d="M230,140 V170" fill="none" stroke="#3b3b3b" stroke-width="2.2" stroke-linejoin="round"/>
<rect x="445" y="45" width="330" height="95" rx="10" fill="#1976d2" stroke="#0d47a1" stroke-width="2"/>
<text x="610.0" y="82.1" text-anchor="middle" font-size="21" font-weight="700" fill="#fff">Análise de tarefas</text>
<text x="610.0" y="102.2" text-anchor="middle" font-size="14" font-weight="400" fill="#fff">Treinar, ver a agenda e</text>
<text x="610.0" y="120.4" text-anchor="middle" font-size="14" font-weight="400" fill="#fff">acompanhar o progresso</text>
<path d="M610,140 V170" fill="none" stroke="#3b3b3b" stroke-width="2.2" stroke-linejoin="round"/>
<rect x="825" y="45" width="330" height="95" rx="10" fill="#1976d2" stroke="#0d47a1" stroke-width="2"/>
<text x="990.0" y="77.5" text-anchor="middle" font-size="21" font-weight="700" fill="#fff">Características da</text>
<text x="990.0" y="104.8" text-anchor="middle" font-size="21" font-weight="700" fill="#fff">plataforma</text>
<text x="990.0" y="125.0" text-anchor="middle" font-size="14" font-weight="400" fill="#fff">Site responsivo: celular e computador</text>
<path d="M990,140 V170" fill="none" stroke="#3b3b3b" stroke-width="2.2" stroke-linejoin="round"/>
<rect x="1205" y="45" width="330" height="95" rx="10" fill="#1976d2" stroke="#0d47a1" stroke-width="2"/>
<text x="1370.0" y="77.5" text-anchor="middle" font-size="21" font-weight="700" fill="#fff">Princípios gerais</text>
<text x="1370.0" y="104.8" text-anchor="middle" font-size="21" font-weight="700" fill="#fff">de projeto</text>
<text x="1370.0" y="125.0" text-anchor="middle" font-size="14" font-weight="400" fill="#fff">Texto grande e linguagem simples</text>
<path d="M1370,140 V170" fill="none" stroke="#3b3b3b" stroke-width="2.2" stroke-linejoin="round"/>
<path d="M230,170 H1370" fill="none" stroke="#3b3b3b" stroke-width="2.2" stroke-linejoin="round"/>
<path d="M800,170 V195" fill="none" stroke="#3b3b3b" stroke-width="2.2" stroke-linejoin="round" marker-end="url(#a)"/>
<rect x="635" y="195" width="330" height="60" rx="10" fill="#1976d2" stroke="#0d47a1" stroke-width="2"/>
<text x="800.0" y="223.7" text-anchor="middle" font-size="21" font-weight="700" fill="#fff">Metas de usabilidade</text>
<text x="800.0" y="243.8" text-anchor="middle" font-size="14" font-weight="400" fill="#fff">Facilidade, clareza e conforto</text>
<rect x="1050" y="195" width="260" height="60" rx="10" fill="#dcdcdc" stroke="#9a9a9a" stroke-width="2"/>
<text x="1180.0" y="224.0" text-anchor="middle" font-size="20" font-weight="700" fill="#333">Guia de estilo</text>
<text x="1180.0" y="242.8" text-anchor="middle" font-size="13" font-weight="400" fill="#333">Cores, fontes e componentes</text>
<path d="M965,225 H1050" fill="none" stroke="#3b3b3b" stroke-width="2.2" stroke-linejoin="round" marker-end="url(#a)"/>
<path d="M800,255 V350" fill="none" stroke="#3b3b3b" stroke-width="2.2" stroke-linejoin="round" marker-end="url(#a)"/>
<g opacity="0.28">
<rect x="20" y="350" width="1560" height="580" rx="20" fill="none" stroke="#0b5a4e" stroke-width="3"/>
<text x="45" y="380" font-size="18" font-weight="700" fill="#0b5a4e">DESIGN, AVALIAÇÃO E DESENVOLVIMENTO</text>
<text x="260" y="416" text-anchor="middle" font-size="17" font-style="italic" font-weight="700" fill="#0b5a4e">nível 1</text>
<text x="800" y="436" text-anchor="middle" font-size="17" font-style="italic" font-weight="700" fill="#0b5a4e">nível 2</text>
<text x="1340" y="436" text-anchor="middle" font-size="17" font-style="italic" font-weight="700" fill="#0b5a4e">nível 3</text>
<rect x="100.0" y="430" width="320" height="72" rx="10" fill="#12806f" stroke="#0b5a4e" stroke-width="2"/>
<text x="260.0" y="463.9" text-anchor="middle" font-size="18" font-weight="700" fill="#fff">Reengenharia do trabalho</text>
<text x="260.0" y="482.7" text-anchor="middle" font-size="13.5" font-weight="400" fill="#fff">Rotina, aulas e agenda em um só lugar</text>
<rect x="100.0" y="526" width="320" height="72" rx="10" fill="#12806f" stroke="#0b5a4e" stroke-width="2"/>
<text x="260.0" y="559.9" text-anchor="middle" font-size="18" font-weight="700" fill="#fff">Projeto do modelo conceitual</text>
<text x="260.0" y="578.7" text-anchor="middle" font-size="13.5" font-weight="400" fill="#fff">Seis seções de navegação</text>
<rect x="100.0" y="622" width="320" height="72" rx="10" fill="#12806f" stroke="#0b5a4e" stroke-width="2"/>
<text x="260.0" y="644.2" text-anchor="middle" font-size="18" font-weight="700" fill="#fff">Protótipos do modelo</text>
<text x="260.0" y="667.6" text-anchor="middle" font-size="18" font-weight="700" fill="#fff">conceitual</text>
<text x="260.0" y="686.4" text-anchor="middle" font-size="13.5" font-weight="400" fill="#fff">Prototipação em papel</text>
<rect x="100.0" y="718" width="320" height="72" rx="10" fill="#12806f" stroke="#0b5a4e" stroke-width="2"/>
<text x="260.0" y="740.2" text-anchor="middle" font-size="18" font-weight="700" fill="#fff">Avaliação iterativa do</text>
<text x="260.0" y="763.6" text-anchor="middle" font-size="18" font-weight="700" fill="#fff">modelo conceitual</text>
<text x="260.0" y="782.4" text-anchor="middle" font-size="13.5" font-weight="400" fill="#fff">Revisão com usuários</text>
<path d="M260,502 V526" fill="none" stroke="#3b3b3b" stroke-width="2.2" stroke-linejoin="round" marker-end="url(#a)"/>
<path d="M260,598 V622" fill="none" stroke="#3b3b3b" stroke-width="2.2" stroke-linejoin="round" marker-end="url(#a)"/>
<path d="M260,694 V718" fill="none" stroke="#3b3b3b" stroke-width="2.2" stroke-linejoin="round" marker-end="url(#a)"/>
<path d="M260,790 V810" fill="none" stroke="#3b3b3b" stroke-width="2.2" stroke-linejoin="round" marker-end="url(#a)"/>
<ellipse cx="260" cy="860" rx="160" ry="50" fill="#12806f" stroke="#0b5a4e" stroke-width="2"/>
<text x="260" y="855.5" text-anchor="middle" font-size="16" font-weight="700" fill="#fff">As principais falhas</text>
<text x="260" y="876.3" text-anchor="middle" font-size="16" font-weight="700" fill="#fff">foram eliminadas?</text>
<path d="M100,860 H60 V466 H100.0" fill="none" stroke="#3b3b3b" stroke-width="2.2" stroke-linejoin="round" marker-end="url(#a)"/>
<text x="46" y="680" text-anchor="middle" font-size="14" font-style="italic" font-weight="700" fill="#3b3b3b" transform="rotate(-90 46 680)">não</text>
<path d="M420,860 H495 V796" fill="none" stroke="#3b3b3b" stroke-width="2.2" stroke-linejoin="round" marker-end="url(#a)"/>
<text x="448" y="852" text-anchor="middle" font-size="14" font-style="italic" font-weight="700" fill="#3b3b3b">sim</text>
<rect x="450" y="740" width="90" height="56" rx="8" fill="#dcdcdc" stroke="#9a9a9a" stroke-width="2"/>
<text x="495.0" y="764.1" text-anchor="middle" font-size="14" font-weight="700" fill="#333">Guia de</text>
<text x="495.0" y="782.3" text-anchor="middle" font-size="14" font-weight="700" fill="#333">estilo</text>
<path d="M495,740 V432 H720 V450" fill="none" stroke="#3b3b3b" stroke-width="2.2" stroke-linejoin="round" marker-end="url(#a)"/>
<rect x="640.0" y="450" width="320" height="72" rx="10" fill="#12806f" stroke="#0b5a4e" stroke-width="2"/>
<text x="800.0" y="483.9" text-anchor="middle" font-size="18" font-weight="700" fill="#fff">Padrões de design de tela</text>
<text x="800.0" y="502.7" text-anchor="middle" font-size="13.5" font-weight="400" fill="#fff">Menus, botões, cartões e textos</text>
<rect x="640.0" y="558" width="320" height="72" rx="10" fill="#12806f" stroke="#0b5a4e" stroke-width="2"/>
<text x="800.0" y="580.2" text-anchor="middle" font-size="18" font-weight="700" fill="#fff">Protótipos dos padrões</text>
<text x="800.0" y="603.6" text-anchor="middle" font-size="18" font-weight="700" fill="#fff">de tela</text>
<text x="800.0" y="622.4" text-anchor="middle" font-size="13.5" font-weight="400" fill="#fff">Esboços das principais telas</text>
<rect x="640.0" y="666" width="320" height="72" rx="10" fill="#12806f" stroke="#0b5a4e" stroke-width="2"/>
<text x="800.0" y="688.2" text-anchor="middle" font-size="18" font-weight="700" fill="#fff">Avaliação iterativa dos</text>
<text x="800.0" y="711.6" text-anchor="middle" font-size="18" font-weight="700" fill="#fff">protótipos de tela</text>
<text x="800.0" y="730.4" text-anchor="middle" font-size="13.5" font-weight="400" fill="#fff">Avaliação heurística</text>
<path d="M800,522 V558" fill="none" stroke="#3b3b3b" stroke-width="2.2" stroke-linejoin="round" marker-end="url(#a)"/>
<path d="M800,630 V666" fill="none" stroke="#3b3b3b" stroke-width="2.2" stroke-linejoin="round" marker-end="url(#a)"/>
<path d="M800,738 V810" fill="none" stroke="#3b3b3b" stroke-width="2.2" stroke-linejoin="round" marker-end="url(#a)"/>
<ellipse cx="800" cy="860" rx="160" ry="50" fill="#12806f" stroke="#0b5a4e" stroke-width="2"/>
<text x="800" y="855.5" text-anchor="middle" font-size="16" font-weight="700" fill="#fff">As metas de usabilidade</text>
<text x="800" y="876.3" text-anchor="middle" font-size="16" font-weight="700" fill="#fff">foram atingidas?</text>
<path d="M640,860 H600 V486 H640.0" fill="none" stroke="#3b3b3b" stroke-width="2.2" stroke-linejoin="round" marker-end="url(#a)"/>
<text x="588" y="680" text-anchor="middle" font-size="14" font-style="italic" font-weight="700" fill="#3b3b3b" transform="rotate(-90 588 680)">não</text>
<path d="M960,860 H1065 V796" fill="none" stroke="#3b3b3b" stroke-width="2.2" stroke-linejoin="round" marker-end="url(#a)"/>
<text x="978" y="852" text-anchor="middle" font-size="14" font-style="italic" font-weight="700" fill="#3b3b3b">sim</text>
<rect x="1020" y="740" width="90" height="56" rx="8" fill="#dcdcdc" stroke="#9a9a9a" stroke-width="2"/>
<text x="1065.0" y="764.1" text-anchor="middle" font-size="14" font-weight="700" fill="#333">Guia de</text>
<text x="1065.0" y="782.3" text-anchor="middle" font-size="14" font-weight="700" fill="#333">estilo</text>
<path d="M1065,740 V432 H1260 V450" fill="none" stroke="#3b3b3b" stroke-width="2.2" stroke-linejoin="round" marker-end="url(#a)"/>
<rect x="1180.0" y="450" width="320" height="72" rx="10" fill="#12806f" stroke="#0b5a4e" stroke-width="2"/>
<text x="1340.0" y="472.2" text-anchor="middle" font-size="18" font-weight="700" fill="#fff">Design detalhado da</text>
<text x="1340.0" y="495.6" text-anchor="middle" font-size="18" font-weight="700" fill="#fff">interface com o usuário</text>
<text x="1340.0" y="514.4" text-anchor="middle" font-size="13.5" font-weight="400" fill="#fff">Alta fidelidade no Figma</text>
<rect x="1180.0" y="546" width="320" height="72" rx="10" fill="#12806f" stroke="#0b5a4e" stroke-width="2"/>
<text x="1340.0" y="568.2" text-anchor="middle" font-size="18" font-weight="700" fill="#fff">Avaliação iterativa do</text>
<text x="1340.0" y="591.6" text-anchor="middle" font-size="18" font-weight="700" fill="#fff">design detalhado</text>
<text x="1340.0" y="610.4" text-anchor="middle" font-size="13.5" font-weight="400" fill="#fff">Teste de usabilidade</text>
<path d="M1340,522 V546" fill="none" stroke="#3b3b3b" stroke-width="2.2" stroke-linejoin="round" marker-end="url(#a)"/>
<path d="M1340,618 V634" fill="none" stroke="#3b3b3b" stroke-width="2.2" stroke-linejoin="round" marker-end="url(#a)"/>
<ellipse cx="1340" cy="676" rx="160" ry="42" fill="#12806f" stroke="#0b5a4e" stroke-width="2"/>
<text x="1340" y="671.8" text-anchor="middle" font-size="15" font-weight="700" fill="#fff">As metas de usabilidade</text>
<text x="1340" y="691.3" text-anchor="middle" font-size="15" font-weight="700" fill="#fff">foram atingidas?</text>
<path d="M1180,676 H1145 V486 H1180.0" fill="none" stroke="#3b3b3b" stroke-width="2.2" stroke-linejoin="round" marker-end="url(#a)"/>
<text x="1133" y="580" text-anchor="middle" font-size="14" font-style="italic" font-weight="700" fill="#3b3b3b" transform="rotate(-90 1133 580)">não</text>
<path d="M1340,718 V742" fill="none" stroke="#3b3b3b" stroke-width="2.2" stroke-linejoin="round" marker-end="url(#a)"/>
<text x="1362" y="734" text-anchor="middle" font-size="14" font-style="italic" font-weight="700" fill="#3b3b3b">sim</text>
<rect x="1295" y="742" width="90" height="44" rx="8" fill="#dcdcdc" stroke="#9a9a9a" stroke-width="2"/>
<text x="1340.0" y="768.8" text-anchor="middle" font-size="13" font-weight="700" fill="#333">Guia de estilo</text>
<path d="M1340,786 V810" fill="none" stroke="#3b3b3b" stroke-width="2.2" stroke-linejoin="round" marker-end="url(#a)"/>
<ellipse cx="1340" cy="860" rx="160" ry="50" fill="#12806f" stroke="#0b5a4e" stroke-width="2"/>
<text x="1340" y="855.8" text-anchor="middle" font-size="15" font-weight="700" fill="#fff">Todas as funcionalidades</text>
<text x="1340" y="875.3" text-anchor="middle" font-size="15" font-weight="700" fill="#fff">foram incluídas?</text>
<path d="M1500,860 H1550 V322" fill="none" stroke="#3b3b3b" stroke-width="2.2" stroke-linejoin="round" marker-end="url(#a)"/>
<text x="1564" y="600" text-anchor="middle" font-size="14" font-style="italic" font-weight="700" fill="#3b3b3b" transform="rotate(-90 1564 600)">não</text>
<path d="M1340,910 V945 H220 V1000" fill="none" stroke="#3b3b3b" stroke-width="2.2" stroke-linejoin="round" marker-end="url(#a)"/>
<text x="1352" y="923" text-anchor="middle" font-size="14" font-style="italic" font-weight="700" fill="#3b3b3b">sim</text>
<rect x="20" y="960" width="1560" height="200" rx="20" fill="none" stroke="#c4561a" stroke-width="3"/>
<text x="45" y="1146" font-size="18" font-weight="700" fill="#c4561a">INSTALAÇÃO</text>
<rect x="100" y="1000" width="240" height="70" rx="10" fill="#ee7d2d" stroke="#c4561a" stroke-width="2"/>
<text x="220.0" y="1033.6" text-anchor="middle" font-size="20" font-weight="700" fill="#fff">Instalação</text>
<text x="220.0" y="1053.0" text-anchor="middle" font-size="13.5" font-weight="400" fill="#fff">Publicação no Figma Sites</text>
<path d="M340,1035 H480" fill="none" stroke="#3b3b3b" stroke-width="2.2" stroke-linejoin="round" marker-end="url(#a)"/>
<rect x="480" y="1000" width="240" height="70" rx="10" fill="#ee7d2d" stroke="#c4561a" stroke-width="2"/>
<text x="600.0" y="1033.6" text-anchor="middle" font-size="20" font-weight="700" fill="#fff">Opinião do usuário</text>
<text x="600.0" y="1053.0" text-anchor="middle" font-size="13.5" font-weight="400" fill="#fff">Coleta de feedback</text>
<path d="M720,1035 H810" fill="none" stroke="#3b3b3b" stroke-width="2.2" stroke-linejoin="round" marker-end="url(#a)"/>
<ellipse cx="1000" cy="1035" rx="190" ry="58" fill="#ee7d2d" stroke="#c4561a" stroke-width="2"/>
<text x="1000" y="1030.5" text-anchor="middle" font-size="16" font-weight="700" fill="#fff">Todas as questões</text>
<text x="1000" y="1051.3" text-anchor="middle" font-size="16" font-weight="700" fill="#fff">foram resolvidas?</text>
<path d="M1190,1035 H1330" fill="none" stroke="#3b3b3b" stroke-width="2.2" stroke-linejoin="round" marker-end="url(#a)"/>
<text x="1260" y="1026" text-anchor="middle" font-size="14" font-style="italic" font-weight="700" fill="#3b3b3b">sim</text>
<ellipse cx="1420" cy="1035" rx="90" ry="36" fill="#e53935" stroke="#b71c1c" stroke-width="2"/>
<text x="1420" y="1042.4" text-anchor="middle" font-size="20" font-weight="700" fill="#fff">Concluído</text>
<path d="M1000,1093 V1115 H720" fill="none" stroke="#3b3b3b" stroke-width="2.2" stroke-linejoin="round" marker-end="url(#a)"/>
<text x="1014" y="1110" text-anchor="middle" font-size="14" font-style="italic" font-weight="700" fill="#3b3b3b">não</text>
<rect x="480" y="1090" width="240" height="52" rx="10" fill="#ee7d2d" stroke="#c4561a" stroke-width="2"/>
<text x="600.0" y="1115.0" text-anchor="middle" font-size="20" font-weight="700" fill="#fff">Melhorias</text>
<text x="600.0" y="1133.8" text-anchor="middle" font-size="13" font-weight="400" fill="#fff">Ajustes na interface</text>
<path d="M600,1090 V1070" fill="none" stroke="#3b3b3b" stroke-width="2.2" stroke-linejoin="round" marker-end="url(#a)"/>
</g>
</g>
</svg>
<img width="1600" height="1250" alt="ciclo-de-vida-requisitos" src="https://github.com/user-attachments/assets/4d5283d7-f231-4a1e-9802-69e928226cc3" />

