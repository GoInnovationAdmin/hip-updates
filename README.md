# Registro de Atualizações — HIP Global Platform

> Histórico de melhorias, correções e novas funcionalidades entregues na plataforma.

---

## 11 de Maio de 2026

### Cadastro mais claro e países traduzidos
A lista de países no cadastro agora respeita o idioma selecionado e a conclusão do cadastro exibe uma mensagem clara antes do login.

### Versão V1.0.11
A versão da plataforma foi atualizada para V1.0.11 após as melhorias no fluxo de cadastro.

### Correção da lista de países no cadastro
A lista de países do cadastro voltou a carregar corretamente e agora possui fallback local para evitar campo vazio em caso de falha temporária da API.

### Versão V1.0.10
A versão da plataforma foi atualizada para V1.0.10 após a correção da lista de países no cadastro.

### Correção no login
A tela de login voltou a carregar sem chamadas indevidas para projetos quando o usuário ainda não está autenticado.

### Versão V1.0.9
A versão da plataforma foi atualizada para V1.0.9 após a correção do login.

### Ajustes de idioma e botão em Projetos
A tela de Projetos passou a usar traduções nos novos textos e o botão de criação agora mostra "Salvar" ao cadastrar um novo projeto.

### Tratamento seguro dos recomendados por projeto
Foi adicionado um tratamento seguro para evitar erro de carregamento ao filtrar recomendações por um projeto recém-criado.

### Versão V1.0.8
A versão da plataforma foi atualizada para V1.0.8 após os ajustes de tradução e recomendados por projeto.

### Ajuste na criação de projetos
Foi corrigido o botão de novo projeto para abrir corretamente o formulário de cadastro.

### Ajuste nos recomendados por projeto
Foi corrigida a exibição de incentivos recomendados para considerar as recomendações já salvas por projeto.

Agora a visão "Todos os projetos" e a visão por projeto individual voltam a exibir oportunidades compatíveis.

### Versão V1.0.7
A versão da plataforma foi atualizada para V1.0.7 após os ajustes na camada de projetos.

### Projetos no perfil do usuário
O antigo Perfil de Correspondência foi evoluído para Projetos.

Agora usuários seekers podem organizar suas informações de correspondência em projetos separados, cada um com briefing, objetivos, países e indústrias alvo próprios.

Os cadastros existentes foram preservados e migrados automaticamente para um projeto inicial chamado "Projeto 1".

### Recomendações por projeto
A tela Explorar Incentivos agora permite filtrar os incentivos recomendados por projeto ou visualizar todos.

Com isso, cada projeto pode ter uma visão própria de oportunidades compatíveis.

### Cadastro com briefing de projeto
No cadastro de usuários seekers, passou a ser obrigatório informar os dados do primeiro projeto, incluindo o briefing do projeto.

Usuários publishers continuam podendo concluir o cadastro sem projeto.

### Versão V1.0.6
A versão da plataforma foi atualizada para V1.0.6 após a entrega da camada de projetos.

### Ajuste nos incentivos recomendados
Foi corrigida a exibição de incentivos recomendados na tela de explorar incentivos.

A plataforma agora evita reutilizar listas vazias em cache e prioriza recomendações válidas já calculadas para o usuário.

### Versão V1.0.5
A versão da plataforma foi atualizada para V1.0.5 após a correção dos recomendados.

## 09 de Maio de 2026

### Versão visível na plataforma
A plataforma agora exibe a versão atual acima do botão "Sair".

A versão é carregada a partir de um arquivo externo de controle e pode ser atualizada sem alterar o código da plataforma.

Quando uma nova versão for detectada, o usuário verá um aviso para recarregar a página.

### Correção de exibição de prazos
Foi corrigida a exibição de datas de prazo dos incentivos para evitar diferença de um dia causada por fuso horário.

Agora a data exibida na visualização permanece igual à data cadastrada ou editada.

### Correção segura dos erros de lint
A base do projeto foi reorganizada para que a verificação de qualidade ignore pastas de referência, backups e arquivos gerados.

Os erros que bloqueavam a validação foram corrigidos sem alterar o funcionamento das telas.

Agora o lint passa sem erros antes do deploy.

## 06 de Maio de 2026

### Incentivos sem valor declarado
Foi adicionada a opção "Incentivo sem valor declarado" no cadastro de incentivos.

Quando marcada, o campo de valor fica bloqueado e a plataforma passa a tratar o incentivo como valor variável.

Nas telas onde o valor do incentivo é exibido, valores variáveis agora aparecem como "Valor variável", com tradução para os idiomas disponíveis.

### Ajuste no cadastro de incentivo
O botão redundante de upload de arquivo foi removido do bloco de links do cadastro de incentivo.

Agora esse bloco é usado apenas para links relacionados, enquanto PDFs do edital e documentos adicionais devem ser enviados pela área de anexos.

### Ajuste na tela de login
A seleção "Qual o seu perfil?" foi removida da tela de login.

Agora o acesso usa apenas e-mail e senha, e a plataforma identifica automaticamente o perfil vinculado à conta.

### Correção no cadastro de usuário
O indicador de etapas do cadastro agora mostra 3 etapas tanto para Pessoa Física quanto para Empresa.

O campo "Qual o seu perfil?" também passou a ser sinalizado como obrigatório.

### Correção na edição de Incentivos Publicados
Foi corrigida a edição de incentivos feita pelo publicador na nova área "Incentivos Publicados".

Agora alterações como país, critérios de elegibilidade, processo de candidatura e website são salvas corretamente.

Também foi ajustada a exibição de datas para evitar diferença de um dia causada por fuso horário.

### Campo de país no cadastro de incentivo
O cadastro de incentivo agora possui o campo de país como informação obrigatória.

Quando o cadastro é iniciado por análise de PDF com IA, a plataforma tenta identificar automaticamente o país do edital e preencher esse campo.

### Feedback visual ao excluir incentivos no Admin
Ao confirmar a exclusão de um incentivo no painel administrativo, o botão agora muda imediatamente para o estado "Deletando...".

Os botões ficam bloqueados durante o processamento, deixando claro que a ação já foi iniciada.

### Correção de data em Incentivos Publicados
Foi corrigida a exibição da data de criação na tela "Incentivos Publicados".

Datas vindas do sistema agora são interpretadas corretamente, evitando a mensagem "Invalid Date".

### Ajustes nas telas do Publisher
As telas "Painel de controle" e "Fluxo de trabalho" do perfil Publisher foram alinhadas com os textos e melhorias visuais já aplicados ao perfil Seeker.

O Publisher agora conta com orientações no painel, textos atualizados e melhor consistência no fluxo de candidaturas.

### Ajuste de indicadores do Publisher
No painel do Publisher, o indicador "Candidaturas recebidas" foi renomeado para "Incentivos adicionados".

O texto de ajuda agora explica que o número representa incentivos do publicador adicionados por usuários ao fluxo de trabalho.

O card "Correspondências Completas" foi removido do painel do Publisher, pois o fluxo passou a ser automático.

### Atualização de textos do fluxo de incentivos
Textos visíveis que ainda mencionavam candidatura, aplicação, aprovação ou rejeição foram revisados para refletir o fluxo atual.

Agora, ao adicionar um incentivo, a comunicação usa termos como "Adicionando incentivo", "Incentivo adicionado" e "Fluxo de trabalho".

### Correção emergencial no login
O login voltou a funcionar corretamente após ajuste na configuração de proteção das senhas para respeitar o limite suportado pelo ambiente de execução.

Com isso, o acesso ao Admin e à lista de incentivos foi normalizado.

### Correção na tela de Incentivos do Admin
A tela de Incentivos do Admin voltou a enviar a autenticação nas chamadas de listagem, visualização, edição, exclusão e upload de PDF.

Isso corrige a mensagem de acesso não autorizado exibida apenas nessa área do Admin.

### Detalhe administrativo do incentivo
A tela de detalhes de incentivo no Admin agora mostra quem cadastrou o incentivo.

Também foi corrigido o carregamento dos dados de "Cadastrado por" e "País" nesse detalhe.

A listagem de incentivos no Admin também passou a mostrar a coluna "Criado por" após a data de cadastro.

Também foi corrigido o envio do nome do cadastrante pela API da listagem, para preencher essa coluna corretamente.

### Ajustes no Painel administrativo
Os textos do dashboard do Admin foram padronizados em português.

Os indicadores também foram renomeados para diferenciar incentivos cadastrados de incentivos adicionados ao fluxo.

O cache interno do dashboard foi renovado para evitar exibição temporária de dados antigos.

Os nomes exibidos nos gráficos de indústrias, países e categorias também foram traduzidos para português.

### Correção no fluxo de trabalho do Seeker
Após adicionar um incentivo, a tela "Fluxo de Trabalho" agora carrega corretamente a visão do Seeker.

Com isso, o incentivo recém-adicionado aparece no card "Meus Incentivos" logo após o redirecionamento.

### Ajuste visual no Fluxo de Trabalho do Seeker
A coluna lateral "Combinações de Incentivos" foi removida da visão Seeker para evitar duplicação com "Meus Incentivos".

O card "Correspondências Completas" foi mantido na tela, mas fica vazio por enquanto.

### Remoção de incentivo pelos meus incentivos
Na página de detalhe de um incentivo já adicionado, agora existe o botão "Remover".

Antes da remoção, o sistema mostra uma confirmação perguntando se o usuário deseja remover o item dos seus incentivos.

### Reforço de segurança das APIs
As APIs administrativas passaram a exigir validação administrativa de forma centralizada.

Também foram reforçadas as regras de origem permitida e os cabeçalhos de segurança das respostas da plataforma.

### Reforço de segurança da sessão
O tempo de sessão foi ajustado para o limite de 30 dias.

Ao sair da plataforma, o acesso também passa a ser encerrado no servidor antes da limpeza local do navegador.

Os limites de tentativas de login, cadastro e recuperação de senha também foram reforçados.

### Reforço de proteção de senhas e arquivos
Novas senhas passam a usar proteção mais forte com salt e múltiplas iterações.

Usuários antigos continuam acessando normalmente, e a proteção da senha é atualizada automaticamente no próximo login bem-sucedido.

O acesso direto a arquivos por caminho no storage também foi reforçado para exigir permissão quando o arquivo não for um documento público de incentivo.

### Revisão dos acessos públicos
Os endpoints públicos necessários para cadastro, configurações públicas e listas auxiliares foram revisados.

A validação pública de códigos afiliados agora retorna apenas as informações necessárias para o cadastro.

Os anexos de incentivos seguem públicos quando pertencem a incentivos visíveis, mas passam a exigir permissão quando o incentivo não estiver público.

### Reforço adicional contra abuso
Uploads, análise de PDF por IA, inscrições de newsletter e validação de códigos afiliados passaram a ter limites específicos de uso.

Uploads de PDF foram restringidos para aceitar apenas arquivos PDF de até 100MB.

Após a redefinição de senha, sessões antigas do usuário passam a ser invalidadas.

Logs detalhados com conteúdo sensível deixam de ser exibidos em produção.

### Ajuste de privacidade no detalhe do incentivo
O nome do usuário que cadastrou o incentivo deixou de aparecer na tela de detalhe do incentivo.

## 05 de Maio de 2026

### Cadastro de edital com múltiplas categorias
O cadastro de incentivo passou a permitir selecionar mais de uma categoria no mesmo edital.

Com isso, um edital pode ser classificado de forma mais completa, sem limitar a apenas uma categoria.

Também foi feita uma atualização de compatibilidade para manter os editais antigos funcionando normalmente durante a transição.

### Ajuste nas opções de "Tipos de Incentivo" criadas no Admin
Foi corrigido o comportamento para que novas opções adicionadas no painel administrativo (como `Prize`/`Prêmio`) apareçam corretamente nos formulários de cadastro e filtros.

Além da atualização em tempo real no backend, também foi ajustado o cache local para reduzir atrasos de atualização no navegador.

### Melhor visual para selecionar múltiplas categorias
O campo de categorias no cadastro de incentivo foi ajustado para mostrar uma lista com marcação individual, facilitando selecionar mais de uma categoria.

As categorias escolhidas agora aparecem como etiquetas abaixo do campo, deixando claro quais opções foram selecionadas.

### Admin e filtros com múltiplas categorias
A edição de incentivo no painel administrativo também passou a aceitar múltiplas categorias.

As telas de busca, filtros e recomendações agora consideram todas as categorias vinculadas ao edital, e não apenas a primeira.

### Tradução de opções no Admin
As opções de categoria, indústria e país no Admin agora respeitam o idioma selecionado.

Isso corrige casos em que etiquetas e filtros apareciam em inglês mesmo com a plataforma em português.

### PDF analisado pela IA salvo como anexo
Ao cadastrar um edital usando a análise por IA, o PDF enviado para leitura agora também fica salvo automaticamente como anexo do edital.

Assim, o documento original analisado permanece disponível junto ao incentivo depois da publicação.

### Anexo obrigatório para publicar edital
A publicação ou edição de um edital agora exige pelo menos um anexo.

Isso garante que todo incentivo publicado tenha um documento de referência disponível para consulta.

### Validação mais clara no cadastro de edital
Quando faltarem campos obrigatórios, a mensagem agora informa quais campos precisam ser preenchidos.

Os campos com problema também passam a ser destacados na tela, facilitando a correção antes de publicar.

### Anexos visíveis no Admin
Ao visualizar ou editar um edital pelo painel administrativo, os anexos cadastrados agora aparecem na tela.

Também foi adicionada a opção de baixar os anexos diretamente pelo Admin.

### Remoção de botão redundante de PDF
Na página de detalhe do edital, o botão separado "Baixar PDF" foi removido.

O download agora fica concentrado na própria lista de anexos, evitando duplicidade na interface.

### Lista de indústrias sem duplicidade
A lista de indústrias no cadastro e edição de edital foi ajustada para não exibir opções repetidas.

As opções continuam traduzidas e organizadas em ordem alfabética.

### Ajustes de nomenclatura em Meus Incentivos
O botão de ação no detalhe do edital agora aparece como "Adicionar aos meus Incentivos".

No Fluxo de Trabalho, a seção de candidaturas do usuário foi renomeada para "Meus Incentivos" e o texto "Seus Alertas" foi removido.

No Painel de Controle, "Correspondências Completas" foi renomeado para "Meus Incentivos", com o texto de apoio "Incentivos que adicionei". O card "Candidaturas enviadas" foi removido para simplificar a experiência.

### Aprovação automática obrigatória de candidaturas
No Admin, a opção "Aprovação automática de candidaturas" agora fica permanentemente marcada e bloqueada para edição.

O backend também força essa configuração como ativa ao salvar configurações, impedindo que a aprovação automática seja desativada por chamada direta de API.

### Otimização de carregamento da lista de incentivos
A lista de incentivos passou a usar cache para reduzir consultas repetidas ao banco de dados.

O cache é atualizado automaticamente quando incentivos são criados, editados, excluídos, expirados ou marcados/removidos como favoritos.

### Otimização do detalhe do incentivo
O detalhe do incentivo agora mantém os dados principais em cache separado dos dados que mudam com frequência.

O registro de visualizações não limpa mais o cache principal do incentivo, melhorando o carregamento em acessos repetidos.

### Otimização do Fluxo de Trabalho e Dashboard
As candidaturas do Fluxo de Trabalho passaram a usar cache temporário para reduzir consultas repetidas ao banco de dados.

O Dashboard e o Fluxo de Trabalho também passaram a carregar informações agrupadas em menos chamadas, tornando a abertura das telas mais eficiente.

As atualizações de perfil, empresa, candidaturas e favoritos agora limpam os caches relacionados automaticamente.

### Otimização do detalhe da candidatura
O detalhe de uma candidatura agora evita uma consulta extra ao banco para identificar o perfil do usuário.

Também foi adicionado cache temporário para acelerar reaberturas do detalhe, com limpeza automática quando a candidatura é aprovada, rejeitada ou excluída.

### Otimização de Incentivos Salvos
A tela de incentivos salvos agora carrega favoritos, candidaturas já adicionadas e o primeiro detalhe em uma única chamada.

Essa mudança reduz chamadas repetidas ao servidor e melhora o tempo de abertura da tela.

### Otimização do detalhe do incentivo
A tela de detalhe do incentivo agora carrega dados do incentivo, status de candidatura e registro de visualização em um fluxo único.

Essa melhoria reduz chamadas separadas ao servidor e deixa a abertura do detalhe mais eficiente.

### Otimização de perfil e empresa
Os dados de perfil do usuário e da empresa agora usam cache temporário seguro por usuário.

Essa melhoria reduz consultas repetidas ao banco ao abrir telas de conta, empresa e carregamentos iniciais do aplicativo.

### Otimização de visualizações de incentivos
O registro de visualizações agora evita gravações repetidas para o mesmo usuário no mesmo incentivo em curto período.

Isso reduz escritas desnecessárias no banco ao reabrir ou atualizar a tela de detalhe do incentivo.

### Invalidação de caches em exclusões de incentivos
As exclusões de incentivos agora identificam usuários afetados por candidaturas, favoritos e publicação antes da remoção.

Após excluir, os caches de dashboard, recomendados, próximos vencimentos e candidaturas desses usuários são atualizados automaticamente.

### Monitoramento de cache
As principais respostas com cache agora indicam se os dados vieram do cache ou se foram carregados novamente.

Essa melhoria ajuda a acompanhar a eficiência das otimizações sem alterar a experiência do usuário.

### Otimização de chamadas nas telas do aplicativo
Algumas telas passaram a reaproveitar melhor dados já carregados no aplicativo, evitando buscas repetidas ao abrir perfil, empresa e fluxo de trabalho.

Essa melhoria reduz chamadas ao servidor e deixa a navegação entre áreas internas mais eficiente.

### Nova área de Incentivos Publicados
Publicadores agora contam com uma nova opção no menu chamada "Incentivos Publicados".

Essa área permite consultar todos os incentivos já publicados, filtrar por indústria, categoria, país, prazo e busca por título, além de visualizar e editar os dados sem acesso à exclusão.

### Lista de candidatos no detalhe do incentivo (Admin)
Na área administrativa, ao abrir os detalhes de um incentivo, agora também aparece a lista de pessoas que se candidataram.

Essa visualização mostra nome, empresa, e-mail, telefone, status e data da candidatura, facilitando o acompanhamento sem precisar abrir outras telas.

### Correção no valor do incentivo com centavos
Foi corrigido o preenchimento do valor no cadastro de incentivo para aceitar formatos como `US$178,00`, sem transformar o valor em zero.

Também foi ajustada a edição posterior, para que o valor salvo possa ser alterado normalmente sem precisar excluir e cadastrar novamente.

### Ajuste nos filtros de Indústria e Categoria em Explorar Incentivos
Foi corrigida a lista de opções dos filtros para evitar itens duplicados e organizar os nomes em ordem alfabética.

Com isso, a navegação ficou mais clara e rápida, sem repetição de opções como `Esportes` e com categorias na ordem correta.


---

## 30 de Abril de 2026

### Administrador pode visualizar a plataforma como Seeker ou Publisher
O usuário administrador agora tem três botões no topo da plataforma:
- **Seeker** — visualiza a plataforma com a experiência de quem busca incentivos
- **Publisher** — visualiza a plataforma com a experiência de quem publica incentivos
- **CMS** — abre o painel administrativo em uma nova aba

Ao clicar em qualquer um dos botões, a página recarrega mostrando os menus e conteúdos corretos para aquela visão.

### Correção: incentivos já candidatados apareciam nas recomendações
Na tela "Explorar Incentivos", a coluna de recomendações mostrava incentivos nos quais o usuário já havia se candidatado. Corrigido: agora apenas incentivos ainda não solicitados aparecem como recomendação.

### Correção: recomendações demoravam para atualizar após candidatura
Após se candidatar a um incentivo, o usuário precisava aguardar alguns minutos para que ele sumisse das recomendações. Agora a atualização acontece imediatamente.

### Atualização na página "Primeiros Passos"
O quarto card da página foi atualizado com um novo conteúdo sobre a IA da plataforma:
- **Título:** "Use nossa IA"
- **Texto:** "Nossa IA te ajuda a preencher todos os dados para a candidatura dos incentivos, fazendo o trabalho pesado pra você."
- O botão deste card foi removido conforme solicitado.
- Atualização aplicada nos três idiomas: Português, Inglês e Espanhol.

---

## 12 de Março de 2026

### Sincronização do código com o repositório oficial
O código da plataforma foi sincronizado com o repositório no GitHub, garantindo que todas as versões estejam alinhadas.

---

## 11 de Fevereiro de 2026

### Ferramenta de preenchimento automático com IA
Lançada a ferramenta de IA para auxiliar na candidatura de incentivos. O usuário faz o upload do edital em PDF e a IA analisa o documento, gera um formulário personalizado e preenche as respostas automaticamente.

### Aprovação automática de candidaturas
Adicionada opção no painel administrativo para aprovar candidaturas automaticamente no momento do envio. Quando ativada, o usuário recebe uma notificação imediata de aprovação.

### Plataforma instalável no celular (PWA)
A plataforma pode agora ser instalada como um aplicativo no celular (iOS e Android), sem precisar de loja de aplicativos. Um botão de instalação é exibido automaticamente para os usuários elegíveis.

---

## Atualizações anteriores

| Data | O que foi feito |
|---|---|
| Fev 2026 | Correção no menu lateral do celular: o menu agora abre pelo lado correto |
| Fev 2026 | Ajuste no cabeçalho do aplicativo no celular: logo à esquerda, menu à direita |
| Fev 2026 | Correção visual no topo da tela em iPhones com notch |
| Fev 2026 | Remoção do modo escuro (dark mode) a pedido |
| Fev 2026 | Sistema de notificações dentro da plataforma, busca por texto nos incentivos e melhorias no fluxo de trabalho |
| Fev 2026 | Plataforma totalmente adaptada para uso no celular |
| Fev 2026 | Exportação de usuários corrigida: exporta todos os registros, não apenas a página atual |
| Fev 2026 | Exportação de dados em formato Excel (.xlsx) no painel administrativo |
| Fev 2026 | "Códigos de Referência" renomeado para "Códigos Afiliados" no painel admin |
| Fev 2026 | Registro de data e hora do último acesso de cada usuário, visível no painel admin |
| Fev 2026 | Página de Afiliados para empresas-mãe: lista de afiliados com funil e detalhes completos |
| Fev 2026 | Campo para associar ou remover código de afiliado ao editar um usuário no admin |
