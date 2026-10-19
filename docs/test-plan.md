# Plano de testes manuais

## Objetivo

Validar a atualização do destino e a manutenção da captura. Os cenários abaixo organizam a validação histórica relatada; não constituem uma nova execução da integração.

## Pré-condições conceituais

Acesso autorizado à configuração e à consulta de leads; rastreamento correspondente localizado; destino correto definido pelo responsável; dados sintéticos para o envio. Nenhum acesso, destino ou dado do atendimento é incluído neste repositório.

| ID | Cenário | Procedimento resumido | Resultado esperado | Resultado relatado |
|---|---|---|---|---|
| TC-01 | Verificar rastreamento ativo | Localizar o rastreamento correspondente e conferir sua configuração | Rastreamento identificado e operacional no fluxo validado | Aprovado |
| TC-02 | Enviar formulário com dados de teste | Preencher e enviar o formulário | Fluxo de envio executado | Aprovado |
| TC-03 | Validar redirecionamento | Observar o destino após o envio | Destino atualizado conforme solicitado | Aprovado |
| TC-04 | Localizar lead registrado | Consultar o cadastro com filtro de e-mail | Registro de teste encontrado | Aprovado |
| TC-05 | Validar fluxo em navegação anônima | Executar o fluxo em sessão anônima | Envio e redirecionamento funcionando nessa sessão | Aprovado |
| TC-06 | Verificar manutenção do endpoint original | Conferir que a intervenção se limitou à configuração de destino | Endpoint original mantido | Aprovado |

Não foram fornecidas datas, versões dos navegadores, matriz de dispositivos ou evidências exportáveis. Não inferimos uma cobertura maior do que a relatada. Navegação anônima reduz influência de uma sessão anterior, mas não simula todos os usuários e ambientes.

## Fora do escopo

Carga, segurança, acessibilidade da landing page real, consentimento, entregabilidade de e-mail, deduplicação, falhas de rede e regressão em múltiplos navegadores. São candidatos a uma etapa futura autorizada, não resultados deste caso.
