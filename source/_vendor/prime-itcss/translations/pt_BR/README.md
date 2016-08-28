# Prime ITCSS

[![licence mit](https://img.shields.io/badge/license-MIT-blue.svg?style=flat-square)](http://hemersonvianna.mit-license.org/)
[![issues](https://img.shields.io/github/issues/prime-solutions/prime-itcss.svg?style=flat-square)](https://github.com/prime-solutions/prime-itcss/issues)
[![GitHub release](https://img.shields.io/github/release/prime-solutions/prime-itcss.svg?style=flat-square)](https://github.com/prime-solutions/prime-itcss/releases)
[![npm](https://img.shields.io/npm/dt/prime-itcss.svg?style=flat-square)](https://www.npmjs.com/package/prime-itcss)
[![devDependency Status](https://img.shields.io/david/dev/prime-solutions/prime-itcss.svg?style=flat-square)](https://david-dm.org/prime-solutions/prime-itcss#info=devDependencies)


## Traduções

* [ORIGINAL](https://github.com/prime-solutions/prime-itcss/)

## Introdução

Com a intenção de se ter um núcleo de CSS de vários projetos em um só lugar. Foi criado esse projeto para servir como base em um projeto front-end. Utilizando a metodologia do [ITCSS](http://itcss.io/) e a sintaxes [SCSS](http://sass-lang.com/), [STYLUS](https://learnboost.github.io/stylus/) e [LESS](http://lesscss.org/).

A ideia de se utilizar o núcleo, se dá quando é necessário ter mais de um projeto no mesmo domínio. Digamos que no seu domínio, terá que haver os arquivos para o site e uma área de admin. Assim, a estrutura com o núcleo ficaria como no exemplo, abaixo:

```
>source
 > prime
 > admin
  > style.scss 
 > site
  > style.scss 
```

Com isso, no `prime` ficaram as ferramentas que serão utilizados em ambos os projetos (ícones, mixins, functions e etc). 

## Exemplo de uso

Em cada pasta de projeto, não será necessário ter algumas pastas (`00-settings, 01-tools, 03-generic, 03-base, 04-vendor e 09-trumps`), mas isso não é uma regra, você saberá o melhor para o seu projeto. 

Ao escrever, estou considerando que os projetos de exemplo (site, admin), são diferentes e por terem essa distinção, as pastas (`05-objetcs, 06-components, 07-pages e 08-theme`), serão personalizadas para cada projeto.

Lembrando mais uma vez, a intenção é mostrar o conceito de que é preciso se ter um `prime`, para evitar código repetido e que dificulte a manutenção. A organização das pastas nos projetos, fica ao critério da necessidade do mesmo.

`style.scss` (site)

```
@import "../prime/00-settings/_variables";
@import "../prime/01-tools/_mixins";

@import "05-objects/_alerts";

```

## Observações e Instalação

O projeto já vem com as sugestões de utilização com o [GulpJS](http://gulpjs.com/) ou [GruntJS](http://gruntjs.com/). Escolhendo um automizador de tarefas, basta saber que só precisa ficar atento em 3 lugares:

- Na raiz, `Gruntfile.js` ou `Gulpfile.js`.
- Na pasta `tasks`, onde as tarefas estão divididas pelo automatizador.
- No arquivo `package.json`, onde estão as dependências.

Se apenas interessa os arquivos, os mesmos se encontram na pasta `source`. Optando por usar um dos automatizadores sugeridos, basta ficar atento aos 3 lugares que foram citados acima e executar no terminal:

```
npm install // Para instalar as dependências
```

E com as dependências instaladas, o comando `default` do automatizador.

## Contribuindo

- Faça o fork!
- Crie a sua branch feature: `git checkout -b my-new-feature`
- Faça o commit das suas alterações: `git commit -m 'Add some feature'`
- Faça o push para o servidor: `git push origin my-new-feature`
- E realize o pull request

## Log

Verifique os [Releases](https://github.com/prime-solutions/prime-itcss/releases) ver detalhado o log de alterações.

## Licença

[MIT license](http://hemersonvianna.mit-license.org/) © Hemerson Vianna
