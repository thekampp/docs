# Kampp — Central de Ajuda

Documentação e tutoriais do **Kampp**, a plataforma onde treinadores acompanham seus alunos, montam treinos e automatizam o dia a dia.

## Estrutura

```
docs.json        Configuração do site (tema, cores, logo, navegação)
icon-512.png     Favicon
logo/            Logo do Kampp
pt-BR/           Tutoriais em português (idioma padrão)
en/              Tutoriais em inglês
```

Cada tutorial é um arquivo `.mdx` e aparece no menu conforme estiver listado em `docs.json` (chave `navigation`).

## Rodar localmente

Instale a CLI da Mintlify (uma vez só):

```bash
npm i -g mint
```

Na raiz do projeto (onde está o `docs.json`), rode:

```bash
mint dev
```

O preview abre em `http://localhost:3000`.

## Publicar (deploy)

O deploy é **automático**: todo `push` na branch `main` é publicado em produção pela Mintlify, que está conectada a este repositório pelo app do GitHub.

```bash
git add -A
git commit -m "Descrição da mudança"
git push
```

## Como adicionar ou editar um tutorial

1. Crie/edite o arquivo `.mdx` na pasta do idioma (`pt-BR/` ou `en/`).
2. Adicione o caminho da página em `docs.json`, no grupo certo (ex.: `"pt-BR/novo-tutorial"`).
3. Confira no `mint dev` e faça o `push`.

> Escreva pensando no treinador: linguagem simples, direta e no passo a passo, sem termos técnicos.

## Problemas comuns

- **Página dá 404:** confira se você está rodando na pasta que tem o `docs.json` e se o caminho foi adicionado na navegação.
- **Ambiente não sobe:** rode `mint update` para atualizar a CLI.

## Links úteis

- [Documentação da Mintlify](https://mintlify.com/docs)
- [Painel da Mintlify](https://dashboard.mintlify.com)
