# Desafio Data Analyst 2026

Este repositório existe apenas para definir as regras da prova e disponibilizar os arquivos iniciais, especialmente [`result.json`](./result.json). A solução final não deve ser desenvolvida aqui.

## Desafio

Crie um robô de scraping que use `result.json` como ponto de partida para buscar e consolidar dados do PNCP e dos portais de compra, gerando uma massa enriquecida e organizada em JSON canônico.

## Regras

1. O candidato deve criar um repositório próprio com os arquivos deste repositório.
2. O repositório da solução deve ser obrigatoriamente privado no GitHub.
3. Se o repositório da solução estiver público em qualquer momento da avaliação, o candidato será eliminado.
4. O candidato deve enviar um convite no GitHub para acesso à solução privada.
5. Este repositório ficará público por 5 dias.
6. O candidato terá 10 dias corridos para concluir o teste.
7. Segurança da informação é requisito fundamental.
8. O uso de IA é permitido.
9. Se utilizar IA, o candidato deve documentar claramente qual ferramenta foi usada e como ela foi aplicada no projeto.

## Requisitos

1. Ler todos os registros de `result.json`.
2. Coletar dados adicionais no PNCP e nos portais de origem.
3. Fazer o merge dos dados com rastreabilidade de fonte.
4. Executar a solução obrigatoriamente via Docker.
5. Salvar a massa de dados em `datasets/`.
6. Salvar os JSONs canônicos finais em `canonicos/`.

## Estrutura Esperada

1. `datasets/`
   Dados brutos, intermediários ou enriquecidos coletados durante o processo.
2. `canonicos/`
   A estrutura interna deve ser definida pelo candidato, desde que seja consistente, auditável e escalável.
3. Como exemplo de nome canônico por arquivo, pode ser usado o padrão:
   `[id_pncp].[portal].[pregao].[unidade_comp].[ano].json`

## Avaliação

1. Qualidade da coleta e ampliação da massa de dados.
2. Qualidade do merge entre PNCP e portais.
3. Organização e consistência dos JSONs canônicos.
4. Performance.
5. Execução via Docker.
6. Clareza do código e da documentação.

## Dicas

1. `pydantic` pode ajudar na modelagem e validação dos dados canônicos.
2. `zendriver` pode ser útil para automação e scraping em portais mais dinâmicos.
3. `typer` pode ajudar a organizar a interface de linha de comando da solução.
4. Essas tecnologias são apenas sugestões. O candidato pode usar qualquer stack.

## Entrega

1. Repositório próprio e privado no GitHub.
2. Convite de acesso para avaliação.
3. Código-fonte da solução.
4. Arquivos de execução via Docker.
5. Um `README.md` bem documentado com instruções de execução, arquitetura, decisões técnicas e uso de IA.
6. Massa de dados em `datasets/`.
7. JSONs finais em `canonicos/`.
