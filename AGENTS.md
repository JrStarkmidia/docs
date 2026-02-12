# Instrucoes do agente de documentacao - StarkMidia

## Contexto do projeto

- Este repositorio contem a documentacao do sistema financeiro da StarkMidia para clientes finais.
- O publico e leigo: pouca familiaridade com sistemas e termos tecnicos.
- O foco e uso pratico do dia a dia: o que existe no sistema e como usar de forma simples.

## Objetivo editorial

- Ensinar tarefas basicas com linguagem clara e direta.
- Reduzir duvidas de primeiro acesso e operacao diaria.
- Priorizar orientacoes acionaveis em vez de explicacoes tecnicas internas.

## Linguagem e tom

- Escreva em portugues do Brasil.
- Fale com o usuario em segunda pessoa: "voce".
- Use voz ativa e frases curtas (uma ideia por frase).
- Evite jargao. Quando um termo tecnico for inevitavel, explique em linguagem simples na mesma secao.
- Use titulos em sentence case.

## Padrao de conteudo por pagina

- Inclua frontmatter com `title` e `description`.
- Abra a pagina com contexto curto: o que a funcionalidade faz e quando usar.
- Traga passo a passo numerado para a tarefa principal.
- Inclua resultado esperado ao final da tarefa.
- Inclua "Proximos passos" com links internos quando fizer sentido.
- Se houver risco de erro comum, adicione um aviso curto com orientacao de correcao.

## Formato e componentes Mintlify

- Use MDX em todas as paginas.
- Prefira componentes nativos do Mintlify (`Card`, `CardGroup`, `Tip`, `Note`, `Warning`, etc.) em vez de HTML puro.
- Referencie elementos de interface em negrito: **Entrar no sistema**, **Salvar**, **Pedidos**.
- Use formato de codigo para comandos, caminhos e arquivos: `npx mint dev`, `docs.json`.
- Em blocos de codigo, sempre use identificador de linguagem quando aplicavel.

## Regras de manutencao

- Verifique `docs.json` antes de qualquer mudanca estrutural ou de navegacao.
- Nao adicione pagina na navegacao se o arquivo ainda nao existir.
- Nao remova paginas sem validar impacto de links internos.
- Preserve o foco em guia de uso; nao transformar paginas em referencia tecnica de API.

## Qualidade e validacao

- Antes de concluir, rodar `npx mint broken-links`.
- Quando houver mudancas relevantes de conteudo ou navegacao, validar no preview com `npx mint dev`.
- Corrigir linguagem para manter leitura simples, escaneavel e sem ambiguidades.

## Definicao de pronto (DoD)

- Cliente leigo consegue entender a funcionalidade sem apoio tecnico.
- A pagina responde: onde clicar, o que preencher e o que esperar.
- O conteudo esta consistente com nomes de menu e fluxo atual do sistema.
