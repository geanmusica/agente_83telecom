# Integrações do Agente 83Telecom

Esta pasta registra como o agente executa ações nos sistemas.

## Ordem obrigatória de execução

1. Usar API oficial quando a ação estiver disponível e documentada.
2. Usar automação de navegador somente quando não houver endpoint adequado.
3. Pedir ação humana quando a operação for crítica, ambígua ou não estiver ensinada.

## Regra de separação

Os procedimentos descrevem **o que fazer**. As integrações descrevem **como executar**.

Exemplo:

- Procedimento: remover etiqueta CLIENTE OFF quando houver autorização e evidência.
- Integração: aplicar ou remover a etiqueta via API do FocusChat, quando possível.

## Segurança

- Nunca salvar tokens, senhas ou credenciais no repositório.
- Usar variáveis de ambiente ou cofre de segredos.
- Registrar a ação realizada, o resultado e eventuais erros sem dados sensíveis.
