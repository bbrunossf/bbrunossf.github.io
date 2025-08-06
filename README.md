# CRIAÇÃO DA PÁGINA DE PORTFOLIO USANDO JEKYLL

## Registrando as etapas
Criei esse arquivo como memória de como foi criada a página, para poder seguir como um guia.  

## Página de portfolio no Github Pages
Optei por usar o Github Pages porque ele pareceu ser simples de usar, para criar um site estático para apresentar os projetos.  
O básico é criar um repositório com o nome 'seu_user'.github.io, criar um arquivo index.html e salvar no repositório.  
O Github Pages tem integração com o Jekyll, que é uma forma de criar a página somente com Markdown, usando templates.

## Jekyll
O Jekyll é feito em Ruby, e acho que tem alguma limitação no Windows, por isso instalei ele no WSL2 na minha máquina local.  
Ao adicionar arquivos md ou html, o Jekyll compila e gera as páginas do site.  
A configuração principal fica no arquivo `_config.yml`, com a definição de título, descrição, tema e outros.  

## Pré-requisitos
Como já dito, o Jekyll precisa do Ruby instalado. Não lembro como instalei.  
Outros pré-requisitos são:  
```sudo apt install build-essential zlib1g-dev libffi-dev libyaml-dev libgdbm-dev libncurses5-dev libreadline-dev libssl-dev```

E a instalação propriamente dita é com
```gem install bundler jekyll```

## O projeto
* criar uma pasta para o projeto;  
* criar um novo site com o Jekyll: ```jekyll new . --force```  ;
* instalar dependências com o Bundler: ```bundle install```  ;
* executar o servidor de desenvolvimento: ```bundle exec jekyll serve```  ;

O acesso é feito na porta local 4000 (eu não lembro de ter feito essa parte, acho que eu só testei vendo o resultado diretamente no link final do github, depois do 'push').  


## Temas
Configurar e usar os temas foi a parte mais difícil, mas vale a pena porque não precisa fazer muita coisa manualmente depois.  
O principal problema foi que alguns temas exigem certos 'plugins', e outros precisam ser compilados ou então copiados na íntegra da fonte e colados corretamente na pasta do projeto.  
Então podemos ter:  
* usar tema pré-configurado (publicado como uma 'gem' no RubyGems) - a princípio, seria só mencionar ele no _config.yml que estaria tudo certo (não usei nenhum assim);  
* usar tema baseado em fonte - copiar manualmente os arquivos do tema para a pasta '_theme' do projeto (os 2 temas que eu testei foram dessa forma;  

### Info extra
no uso de um determinado tema, tive que instalar um 'gem' que era pré-requisito dele, adicionando a linha no arquivo 'gemfile':
```gem "kramdown-parser-gfm"```  
É preciso ficar atento aos pré-requisitos do tema, e também o que o tema traz de layouts que podem ser usados, caso queira uma formatação/layout diferente para cada tipo de página (um layout para a página central, outro estilo para posts, etc).  
Layout é um arquivo com base de HTML com 'hooks' como se fossem variáveis, que são populadas com as informações do arquivo .md (daí a necessidade de uma estrutura mínima para os arquivos md).


## Estrutura mínima dos arquivos .md


## Minha página
Como eu queria uma página inicial com links para os projetos, usei formatação com Markdown e HTML para ficar mais bonito, dentro de um layout de tema usado.  
O conteúdo HTML foram a tag 'h1' para o título, a descrição css dos cards na tag 'style', um 'div' geral para comportar os cards, e um 'div class="card'' para cada card/projeto.  
```
---
layout: default
title: Projetos
permalink: /projetos/
---

<h1>💼 Meus Projetos</h1>

<style>
.grid {
  display: grid;
  grid-template-columns: repeat(auto-fit, minmax(250px, 1fr));
  gap: 1.5rem;
  margin-top: 2rem;
}
.card {
  border: 1px solid #ccc;
  border-radius: 8px;
  padding: 1rem;
  background: #fff;
  box-shadow: 2px 2px 6px rgba(0,0,0,0.1);
  transition: transform 0.2s;
}
.card:hover {
  transform: translateY(-5px);
}
.card-title {
  font-size: 1.2rem;
  font-weight: bold;
}
.card-desc {
  margin: 0.5rem 0;
  font-size: 0.95rem;
}
.card-link {
  text-decoration: none;
  color: #1a73e8;
}
</style>

<div class="grid">

  <div class="card">
    <div class="card-title">📊 Análise de Vendas 2024</div>
    <div class="card-desc">
      Análise de dados de vendas com Pandas e visualizações com Matplotlib.
    </div>
    <a class="card-link" href="https://github.com/seu-usuario/analise-vendas" target="_blank">Ver no GitHub</a>
  </div>

  <div class="card">
    <div class="card-title">📈 Previsão com Prophet</div>
    <div class="card-desc">
      Estudo de séries temporais com Prophet aplicado a dados reais.
    </div>
    <a class="card-link" href="https://github.com/seu-usuario/previsao-prophet" target="_blank">Ver no GitHub</a>
  </div>

  <div class="card">
    <div class="card-title">📉 Dashboard de BI</div>
    <div class="card-desc">
      Dashboard interativo criado com Streamlit para análise executiva.
    </div>
    <a class="card-link" href="https://github.com/seu-usuario/streamlit-dashboard" target="_blank">Ver no GitHub</a>
  </div>

</div>

```

## Resumo
* Instalar o Ruby;  
* Instalar os pré-requisitos do Jekyll;  
* Instalar Jekyll e Bundler;  
* Criar novo site usando Jekyll;  
* Clonar o repositório via ssh (para não dar erro da WSL2);  
* Editar o conteúdo nos arquivos Markdown;  
* Gerar o site localmente e atualizar o Github (usei uma branch 'master' ao invés de 'main');  
* Copiar o conteúdo da pasta '_site/' (resultado da compilação feita pelo Jekyll) para a raiz da branch;  
* Fazer o git add, commit e push;  
* Nos settings do Github, configurar a branch como fonte;  

### Para futuras atualizações:
* Editar os arquivos .md;  
* Executar os comandos:  
```
bundle exec jekyll build
git add .
git commit -m "Atualização"
git push origin gh-pages
```

### Fontes
https://emojipedia.org/  
https://github.com/ikatyang/emoji-cheat-sheet  
