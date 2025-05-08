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
    <div class="card-title">📉 Agente PPT</div>
    <div class="card-desc">
      Utiliza um Agente de IA para demonstrar algumas funções em uma apresentação ao vivo.
    </div>
    <a class="card-link" href="https://github.com/bbrunossf/presentationAgent" target="_blank">Ver no GitHub</a>
  </div>

</div>

