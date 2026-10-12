---
layout: default
title: Projetos
permalink: /
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
    <div class="card-title">📊 Sistema de Controle de custos de um escritório de Engenharia</div>
    <div class="card-desc">
      Sistema para apontamento de horas gastas por projetos em um escritório de Engenharia.  
       Backend em python, frontend em Remix
    </div>
    <a class="card-link" href="https://github.com/bbrunossf/plena" target="_blank">Ver no GitHub</a>
  </div>

  <div class="card">
    <div class="card-title">📈 Análise de Ativos no Mercado Financeiro</div>
    <div class="card-desc">
      Painel para estudos dos preços dos ativos para auxiliar na decisão de investimentos.
       Frontend em Streamlit / Dash, com gráficos dos ativos e indicadores técnicos.
    </div>
    <a class="card-link" href="https://github.com/bbrunossf/trendfollow" target="_blank">Ver no GitHub</a>
  </div>

  <div class="card">
    <div class="card-title">📢 Agente PPT</div>
    <div class="card-desc">
      Utiliza um Agente de IA para demonstrar algumas funções em uma apresentação ao vivo.
    </div>
    <a class="card-link" href="https://github.com/bbrunossf/presentationAgent" target="_blank">Ver no GitHub</a>
  </div>
  
  <div class="card">
    <div class="card-title">🎵 Music Player Tube</div>
    <div class="card-desc">
      Cria uma interface web para pesquisar termos em playlists do YouTube, com a opção de baixar todos os vídeos ou somente alguns vídeos selecionados para download. Baixa os arquivos em uma pasta de mídia do Jellyfin, ficando disponíveis para reprodução (sem anúncios).  
	  Backend: Python com yt_dlp em um container Docker  
	  Frontend: framework Remix
    </div>
    <a class="card-link" href="https://github.com/bbrunossf/music_player_tube" target="_blank">Ver no GitHub</a>
  </div>
<div class="card">
    <div class="card-title"> Dashboard com PowerBI - Custos de um Escritório de Engenharia</div>
    <div class="card-desc">
      Um Dashboard com 3 visões diferentes para apresentar e analisar dados de custos de um escritório de projetos de Engenharia Civil, utilizando PowerBI.
    </div>
    <a class="card-link" href="https://github.com/bbrunossf/dash_powerbi_01" target="_blank">Ver no GitHub</a>
  </div>

  <div class="card">
    <div class="card-title">🖊️ Croqui técnico convertido em DXF</div>
    <div class="card-desc">
      Converte croquis de engenharia desenhados à mão em arquivos DXF: o desenho é ajustado a
      templates paramétricos e o posicionamento é resolvido por solver geométrico.
      Backend em Python (FastAPI), frontend em React.
    </div>
    <a class="card-link" href="https://github.com/bbrunossf/croqui2dxf" target="_blank">Ver no GitHub</a>
  </div>

  <div class="card">
    <div class="card-title">🍽️ Cardápio Hospitalar (NutriClin)</div>
    <div class="card-desc">
      Sistema web de planejamento nutricional hospitalar: catálogo de pratos e ingredientes,
      regras de dietas e geração de cardápios por otimização matemática (PuLP/CBC),
      com planos nutricionais por paciente.
    </div>
    <a class="card-link" href="https://github.com/bbrunossf/cardapio_hospitalar2026" target="_blank">Ver no GitHub</a>
  </div>

  <div class="card">
    <div class="card-title">🧱 Orça Obras - Orçamento a partir do SINAPI</div>
    <div class="card-desc">
      Lê a planilha SINAPI e monta o orçamento da obra: o usuário seleciona os serviços por grupo
      e informa as quantidades, e o sistema devolve a tabela de custos.
      Python.
    </div>
    <a class="card-link" href="https://github.com/bbrunossf/orcaobras" target="_blank">Ver no GitHub</a>
  </div>

  <div class="card">
    <div class="card-title">📄 Geração de GRDs - Guias de Remessa de Documentos</div>
    <div class="card-desc">
      Emissão de Guias de Remessa de Documentos, com backend Flask modularizado --
      refatorado de uma versão anterior em Streamlit para permitir a edição dos dados tabulares.
    </div>
    <a class="card-link" href="https://github.com/bbrunossf/novagrd" target="_blank">Ver no GitHub</a>
  </div>

  <div class="card">
    <div class="card-title">💬 Gerenciador de conversas do ChatGPT</div>
    <div class="card-desc">
      Aplicação React que abre o arquivo de conversas exportado do ChatGPT: busca, ordenação,
      tags, exclusão em massa e exportação. Roda inteiramente no navegador, sem backend, e abre
      com dados de exemplo para demonstração imediata.
    </div>
    <a class="card-link" href="https://github.com/bbrunossf/chatmanager" target="_blank">Ver no GitHub</a>
  </div>

  <div class="card">
    <div class="card-title">🎙️ Assistente de voz em tempo real</div>
    <div class="card-desc">
      Conversa por voz em fluxo contínuo no navegador, usando a Realtime API: sem o encadeamento
      gravar &#8594; transcrever &#8594; responder &#8594; sintetizar.
      Backend em FastAPI.
    </div>
    <a class="card-link" href="https://github.com/bbrunossf/voice-assistant" target="_blank">Ver no GitHub</a>
  </div>

  <div class="card">
    <div class="card-title">📚 Interface para trabalhar com arquivos de um projeto</div>
    <div class="card-desc">
      Lista de arquivos (PDF) à esquerda, pré-visualização no centro e painel de notas à direita,
      no estilo do NotebookLM. TypeScript.
    </div>
    <a class="card-link" href="https://github.com/bbrunossf/notebookLM" target="_blank">Ver no GitHub</a>
  </div>

  <div class="card">
    <div class="card-title">📅 Cronograma Gantt com integração Trello</div>
    <div class="card-desc">
      Cronograma em Gantt (frappe-gantt) com projetos e tarefas em PostgreSQL via Prisma,
      importação de tarefas do Trello e sincronização de progresso. React Router.
    </div>
    <a class="card-link" href="https://github.com/bbrunossf/gantt-app" target="_blank">Ver no GitHub</a>
  </div>

  <div class="card">
    <div class="card-title">🗳️ Painel de avaliação de candidatos - Eleições ES 2026</div>
    <div class="card-desc">
      Painel Streamlit que compara os candidatos do Espírito Santo que já ocupam cargo
      (33 deputados estaduais e 10 federais) em quatro dimensões de avaliação. Python.
    </div>
    <a class="card-link" href="https://github.com/bbrunossf/eleicoes2026" target="_blank">Ver no GitHub</a>
  </div>

  <div class="card">
    <div class="card-title">🕸️ Este portfólio como grafo interativo</div>
    <div class="card-desc">
      Os projetos, ferramentas e conhecimentos deste portfólio apresentados como um grafo
      navegável: dois layouts, busca e visão essencial ou completa. React + Cytoscape.
    </div>
    <a class="card-link" href="https://github.com/bbrunossf/portfolio_em_grafo" target="_blank">Ver no GitHub</a>
    &nbsp;·&nbsp;
    <a class="card-link" href="https://bbrunossf.github.io/portfolio_em_grafo/" target="_blank">Abrir o grafo</a>
  </div>

  <div class="card">
    <div class="card-title">🎧 Transcrição de áudios em texto para LLMs</div>
    <div class="card-desc">
      Ferramenta web que transcreve arquivos de áudio em arquivos de texto simples, no formato
      adequado para alimentar modelos de linguagem. Aplicação Flask com arquitetura modular
      (blueprints e camada de serviços), integrada à API da AssemblyAI, com painel das
      transcrições salvas e download.
    </div>
    <a class="card-link" href="https://github.com/bbrunossf/flask-audio-transcription" target="_blank">Ver no GitHub</a>
  </div>
</div>

