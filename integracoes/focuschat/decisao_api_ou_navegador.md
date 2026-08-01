# Decisão: API ou navegador no FocusChat

Antes de executar uma ação no FocusChat, o agente deve seguir esta decisão.

## 1. A ação existe na API e foi validada?

- **Sim:** usar a API.
- **Não:** seguir para a etapa 2.

## 2. Existe um procedimento de navegador ensinado e testado?

- **Sim:** usar o navegador seguindo exatamente o procedimento.
- **Não:** não improvisar; informar que a ação ainda precisa ser ensinada ou executada por uma pessoa.

## 3. A ação altera dados ou afeta o cliente?

Confirmar que existe autorização dentro do escopo atual antes de executar.

## Confirmação após a ação

Depois de executar:

1. Validar se o resultado esperado realmente ocorreu.
2. Registrar sucesso ou falha sem expor dados sensíveis.
3. Verificar se surgiu aprendizado operacional novo e reutilizável.
4. Quando houver aprendizado confirmado, atualizar o arquivo correto no GitHub.

## Regra contra improvisação

A IA pode escolher uma habilidade conhecida, mas não deve inventar endpoints, parâmetros, botões, caminhos ou resultados.
