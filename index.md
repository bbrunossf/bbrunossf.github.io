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

