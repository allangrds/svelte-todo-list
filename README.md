# Svelete - Todo list

## Sumário

- [Requisitos](#requisitos)
- [Instalação](#instalação)
- [Uso](#uso)
- [Build](#build)
- [Commits](#commits)

## Requisitos

- Node v12.18.2
- Npm v6.14.8

## Instalação

Execute o seguindo comando no seu terminal:

```bash
npm install
```

## Uso

Execute o seguindo comando no seu terminal:

```bash
npm start
```

## Build

Para gerar a versão de produção execute o seguindo comando no seu terminal:

```bash
npm run build
```

## Commits

O desenvolvimento desse Todolist foi dividido em 3 partes, tendo todos eles o mesmo resultado:

1. Usando o componente `List` a partir do `Todo`, passando diretamente como prop.

2. Usando o componente `List` a partir do container `App`, e removendo parte da função `addTasks` do `Todo` para o container.

3. Fazendo uso da store do Svelte - semelhante ao gerenciamente de estado global que temos no React.