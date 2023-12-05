## Setup

Verifica se tu tem algum versionador de node instalado na máquina. Pode ser o classico [nvm](https://github.com/nvm-sh/nvm) ou um mais moderninho como o [fnm](https://github.com/Schniz/fnm) ou só baixa a versao mesmo 

ve se tu tem node 18 instalado

```bash
nvm use
```

se não tiver, rode o comando

```bash
nvm install
```

proximo

baixa o pnpm. pnpm é um package manager de javascript é tipo npm mas é mais rapido, vai por mim

```bash
npm i -g pnpm
```

é pra ta tudo pronto

qualquer coisa pesquisa

## Start do projeto

instale as dependências:

```bash
pnpm i
```

rode o server de desenvolvimento:

```bash
pnpm dev
```

abre algum browser (eu recomendo o chrome por causa das developer tools q eu acho mais agradaveis) nessa url [http://localhost:3000](http://localhost:3000)

tu pode começar a mexer no codigo em `/src`

## estrutura do projeto
```bash
.
src
├── app
│   ├── rota ## cada diretorio dentro de `/app/` é uma `/rota`
│   │   └── page.js ## page é o nome do arquivo q serve a ui da rota
│   ├── api
│   │   └── route.js ## route é o arquivo responsavel por servir metodos http (cominicaçao com o back)
│   ├── layout.js ## estrutura compartilhada entro paginas
│   └── page.js ## home do app
│   ├── components
│   │   ├── ui ## componetes primitivos
│   │   │   ├── alert-dialog.js
│   │   │   ├── button.js
│   │   │   ├── dropdown-menu.js
│   │   │   └── ...
│   │   ├── main-nav.js ## componets compostos 
│   │   ├── page-header.js ## componets compostos
│   │   └── ...
│   ├── lib
│   │   └── utils.ts ## funcoes compartilhadas
│   └── styles
│       └── globals.css
├── next.config.js ## configs (provavelmente tu n vai mexer nelas)
├── package.json
├── postcss.config.js
├── tailwind.config.js
└── tsconfig.json
```

## Ta perdido e n sabe oq fazer?

- [docs react](https://react.dev/)
- [docs next](https://nextjs.org/docs)
- [docs tailwind](https://tailwindcss.com/docs/installation)
- [shadcn ui (lib de componentes)](https://ui.shadcn.com/docs)

## Videos inspiracionais
- [video q fez eu entender react rerver components](https://www.youtube.com/watch?v=zMf_xeGPn6s)
- [react core team falando sobre novas features](https://www.youtube.com/watch?v=g5BGoLyGjY0&t=1162s)
- [como next funciona](https://www.youtube.com/watch?v=d2yNsZd5PMs&t=360s)
- [tailwind na pratica](https://www.youtube.com/watch?v=pfaSUYaSgRo&t=65s&pp=ugMICgJwdBABGAHKBQh0YWlsd2luZA%3D%3D)
- [shadcn ui e pq é tao foda](https://www.youtube.com/watch?v=dD1fpoGHuC8)
