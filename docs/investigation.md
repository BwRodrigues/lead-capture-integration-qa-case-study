# Investigação

## Escopo e origem do relato

Este documento resume a experiência manual informada pelo autor. Os exemplos foram recriados de forma genérica. Não disponibilizamos artefatos privados para comprovar ou reproduzir o atendimento.

## Observado, testado e confirmado

| Etapa | Natureza da evidência relatada | Resultado |
|---|---|---|
| Inspeção do HTML | Observação | Método POST e endpoint identificados |
| Consulta do domínio e CNAME | Investigação | Subsídio para identificar a plataforma responsável |
| Localização do rastreamento | Observação na plataforma | Configuração correspondente localizada |
| Mudança do destino | Manutenção de configuração | URL de redirecionamento atualizada na plataforma |
| Envio em navegação anônima | Teste manual | Fluxo executado e destino correto observado |
| Busca por e-mail | Verificação manual | Lead de teste localizado na plataforma |

## Hipóteses descartadas ou não confirmadas

A necessidade de modificar o HTML ou o DNS foi uma possibilidade investigada, não uma mudança executada. O resultado relatado dispensou essas alterações.

A listagem inicial não mostrava o cadastro esperado. A hipótese de falha de captura perdeu sustentação após localizar o lead pelo filtro de e-mail. A causa da ausência visual inicial não foi determinada; não atribuímos o episódio a um bug ou atraso.

## Limites técnicos

POST descreve o método de envio, mas não prova persistência. CNAME é um alias de DNS e não informa, por si só, a lógica da aplicação. Redirecionamento bem-sucedido não prova que um cadastro foi salvo. Por isso, a verificação do registro foi uma etapa independente.

Não há relato de análise de payloads, códigos HTTP, cabeçalhos, tráfego de rede via DevTools ou testes automatizados. Nenhum comando DNS com dados reais é incluído.
