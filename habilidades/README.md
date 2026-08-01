# Habilidades do Agente 83Telecom

Este arquivo registra o que o agente pode fazer e o nível de prontidão de cada habilidade.

## Estados

- `[ ]` Não ensinada.
- `[~]` Procedimento documentado, mas ainda não testado.
- `[x]` Testada e liberada para uso.

Uma habilidade só pode ser marcada como `[x]` depois de existir procedimento claro, validação do resultado e teste real autorizado.

## FocusChat

- [ ] Assumir atendimento
- [ ] Responder cliente
- [ ] Transferir atendimento para outro setor
- [ ] Colocar atendimento em aguardando
- [ ] Finalizar chat
- [ ] Adicionar etiqueta
- [ ] Remover etiqueta
- [ ] Enviar mensagem interna por sussurro
- [~] Localizar cliente e atendimento aberto

## SGP

- [~] Consultar cliente
- [ ] Consultar contrato
- [~] Consultar ONU coletiva
- [~] Consultar clientes com fibra individual
- [~] Verificar sinal óptico, RSSI e potência óptica
- [ ] Consultar financeiro
- [ ] Abrir ocorrência
- [~] Abrir OS após diagnóstico e verificação de duplicidade
- [~] Agendar visita
- [~] Finalizar OS e chat
- [ ] Alterar nome da rede Wi-Fi

## Supervisão

- [ ] Revisar fila Manual
- [ ] Identificar clientes aguardando atendente
- [ ] Detectar atrasos e casos críticos
- [ ] Comparar etiqueta CLIENTE OFF com o status no SGP
- [ ] Gerar resumo de supervisão

## Aprendizado e documentação

- [x] Verificar se houve aprendizado novo após cada interação
- [x] Separar informação permanente de informação temporária
- [x] Atualizar o arquivo correto no GitHub
- [x] Não registrar senhas, tokens, credenciais ou dados temporários de clientes
- [x] Criar ou atualizar procedimento quando houver conhecimento operacional novo e confirmado

## Regra de execução

Antes de executar uma tarefa, o agente deve consultar este catálogo:

1. Se estiver `[x]`, executar seguindo o procedimento correspondente.
2. Se estiver `[~]`, somente executar com supervisão e autorização direta.
3. Se estiver `[ ]`, não improvisar; solicitar treinamento ou instrução.
4. Ao concluir, executar o ciclo descrito em `regras/ciclo_de_aprendizado.md`.
