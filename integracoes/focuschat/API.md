# API do FocusChat

Documentação oficial analisada: API de integração do FocusChat.

## Autenticação

As requisições usam o cabeçalho `access-token`, contendo o token do canal.

O token é secreto e não deve ser registrado neste repositório.

## Capacidades úteis já identificadas

### Contatos

- Buscar contato por ID.
- Buscar contato pelo número.
- Listar e filtrar contatos.
- Editar dados do contato.
- Consultar as etiquetas vinculadas ao contato.
- Adicionar etiquetas sem remover as existentes.

### Atendimentos e chats

- Buscar atendimentos por estado, setor, usuário, contato, número, protocolo e período.
- Consultar atributos de um chat.

Estados documentados para consulta de atendimentos:

- `0`: automático
- `1`: aguardando
- `2`: manual
- `3`: finalizado
- `4`: pesquisa de satisfação
- `5`: fora de hora

### Estrutura da operação

- Listar setores.
- Listar usuários e consultar seu estado.
- Consultar tags.
- Criar, editar e excluir tags administrativas.
- Consultar respostas rápidas.

## Uso recomendado pelo agente

Priorizar a API para:

- localizar clientes e atendimentos;
- consultar filas e estados;
- consultar setores e usuários;
- consultar dados e etiquetas de contatos;
- adicionar etiquetas quando a ação estiver autorizada;
- obter atributos necessários ao fluxo.

## Atenção

Criar, editar ou excluir uma tag da organização é diferente de adicionar uma tag já existente a um contato. Alterações administrativas exigem autorização específica.

A documentação deve ser validada novamente antes da implementação, pois endpoints, campos e limites podem mudar.
