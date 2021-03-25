---
layout: post
title:  "Como eu fiz essa página?"
date:   2021-03-24 18:10:00 -0300
categories: tech github.io
tags: [Jekyll, github.io, Yaml, Ruby, Jekyll, Github Actions, Github]
---

Esta página foi feita utilizando o Jekyll, que segundo sua própria definição é capaz de transformar texto plano em sites estáticos e blogs. É possível gerar páginas com html, css, js normalmente e também é possível utilizar markdown. Tudo isso e ainda é possíveis utilizar [***variáveis pré definidas***](https://jekyllrb.com/docs/variables/) graças ao [***Liquid templating system***](https://github.com/Shopify/liquid/wiki/Liquid-for-Designers). Muito legal!
<br/>

## Hospedagem
Esta página é hospedada graças ao [***Github Pages***](https://pages.github.com/). Você consegue fazer tudo de forma automática, utilizando algum dos [***temas disponíveis***](https://pages.github.com/themes/). Porém como eu nunca havia tido contato com Ruby, Jekyll e havia gostado do tema [***Chirpy***](https://github.com/cotes2020/jekyll-theme-chirpy), que não está disponível no modo "wizard", então resolvi fazer da maneira mais manual para conhecer melhor essas ferramentas e poder usar o tema.

## O que eu fiz?
De forma bem resumida foi: 
- 1º e mais importante: ví a série de vídeos disponível no item [**tutorial**](#tutorial)
- instalei o [***Ruby***](https://rubyinstaller.org/downloads/) na minha máquina;
- depois o [***Jekyll***](https://jekyllrb.com/);
- fiz um fork do tema;
- renomiei o repositório para (**[NOME_SITE].github.io**);
- clonei tudo pra minha máquina;
- alterei algumas informações no template;
- após o primeiro push que você fizer o [***Github Actions***](https://github.com/features/actions) irá executar os passos definidos em [***Yaml***](https://yaml.org/) no arquivo ".github/workflows/pages-deploy.yml". Um branch será gerado com o nome **gh-pages**. Nas configurações do repositórios deve-se alterar para exibir as páginas a partir deste branch.

Pronto, o site está no ar! 

## Tutorial
Na verdade tudo que está resumido aqui está muito melhor explicado numa série de 19 vídeos no Youtube chamada [***Jekyll - Static Site Generator | Tutorial***](https://www.youtube.com/watch?v=T1itpPvFWHI&list=PLLAZ4kZ9dFpOPV5C5Ay0pHaa0RJFhcmcB). Recomendo.

## Comandos úteis (para rodar local)
Criar um novo blog/site:
{% highlight ruby %}
jekyll new NOME_BLOG
{% endhighlight %}
Executar o site:
{% highlight ruby %}
bundle exec jekyll serve
{% endhighlight %}

