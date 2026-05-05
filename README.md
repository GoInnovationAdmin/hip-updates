# Registro de Atualizações — HIP Global Platform

> Histórico de melhorias, correções e novas funcionalidades entregues na plataforma.

---

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
