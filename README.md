<!DOCTYPE html>
<html lang="pt-BR">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0">

<title>MOC — Mapa de Oportunidades Culturais</title>

<meta name="description" content="MOC — Mapa de Oportunidades Culturais">

<style>

/* =========================
   CONFIGURAÇÕES GERAIS
========================= */

:root {
    --roxo: #6f2dbd;
    --roxo-escuro: #3f176f;
    --lilas: #f4edff;
    --lilas-2: #e8d8ff;
    --texto: #25202d;
    --branco: #ffffff;
    --cinza: #6e6878;
    --borda: #e3d8ef;
    --sombra: 0 12px 35px rgba(63,23,111,.10);
}

* {
    box-sizing: border-box;
    margin: 0;
    padding: 0;
}

html {
    scroll-behavior: smooth;
}

body {
    font-family: Arial, Helvetica, sans-serif;
    color: var(--texto);
    background: white;
    line-height: 1.6;
}

a {
    text-decoration: none;
    color: inherit;
}

.container {
    width: min(1120px, 92%);
    margin: auto;
}


/* =========================
   MENU
========================= */

nav {
    position: sticky;
    top: 0;
    z-index: 20;
    background: rgba(255,255,255,.94);
    backdrop-filter: blur(10px);
    border-bottom: 1px solid var(--borda);
}

.nav-inner {
    min-height: 70px;
    display: flex;
    align-items: center;
    justify-content: space-between;
}

.logo {
    display: flex;
    align-items: center;
    gap: 10px;
    font-weight: 800;
    color: var(--roxo);
}

.logo-mark {
    width: 42px;
    height: 42px;
    border-radius: 12px;
    background: var(--roxo);
    color: white;
    display: grid;
    place-items: center;
    font-size: 21px;
    font-weight: 900;
}

.nav-links {
    display: flex;
    gap: 24px;
    font-size: 14px;
    font-weight: 700;
}

.nav-links a:hover {
    color: var(--roxo);
}

.menu {
    display: none;
    border: 0;
    background: none;
    font-size: 28px;
    color: var(--roxo);
}


/* =========================
   CAPA
========================= */

.hero {
    background:
        radial-gradient(
            circle at 85% 15%,
            #d9baff 0,
            transparent 27%
        ),
        linear-gradient(135deg,#fbf8ff,#eee1ff);

    padding: 85px 0 70px;
}

.hero-grid {
    display: grid;
    grid-template-columns: 1.15fr .85fr;
    gap: 55px;
    align-items: center;
}

.badge {
    display: inline-block;
    background: var(--lilas-2);
    color: var(--roxo-escuro);
    padding: 7px 13px;
    border-radius: 999px;
    font-size: 13px;
    font-weight: 800;
    margin-bottom: 18px;
}

h1 {
    font-size: clamp(42px,6vw,72px);
    line-height: 1.02;
    letter-spacing: -2px;
}

.gradient {
    color: var(--roxo);
}

.hero p {
    font-size: 19px;
    color: #554d60;
    max-width: 650px;
    margin: 22px 0;
}

.btn {
    display: inline-block;
    background: var(--roxo);
    color: white;
    padding: 13px 20px;
    border-radius: 12px;
    font-weight: 800;
    box-shadow: 0 8px 20px rgba(111,45,189,.22);
}

.btn:hover {
    background: var(--roxo-escuro);
}

.hero-card {
    background: white;
    border: 1px solid var(--borda);
    border-radius: 28px;
    padding: 28px;
    box-shadow: var(--sombra);
}

.hero-card h3 {
    color: var(--roxo);
    margin-bottom: 15px;
}

.flow {
    display: grid;
    gap: 10px;
}

.flow-item {
    display: flex;
    align-items: center;
    gap: 12px;
    padding: 12px;
    border-radius: 13px;
    background: #faf7ff;
    border: 1px solid #eee3fa;
    font-weight: 700;
}

.icon {
    width: 36px;
    height: 36px;
    border-radius: 10px;
    background: var(--lilas-2);
    color: var(--roxo);
    display: grid;
    place-items: center;
    font-weight: 900;
}


/* =========================
   SEÇÕES
========================= */

section {
    padding: 78px 0;
}

.section-title {
    text-align: center;
    max-width: 760px;
    margin: 0 auto 42px;
}

.section-title span {
    color: var(--roxo);
    font-weight: 800;
    text-transform: uppercase;
    font-size: 13px;
}

.section-title h2 {
    font-size: clamp(30px,4vw,44px);
    line-height: 1.1;
    margin: 8px 0 12px;
}

.section-title p {
    color: var(--cinza);
}


/* =========================
   PROBLEMA
========================= */

.problem {
    display: grid;
    grid-template-columns: 1fr 1fr;
    gap: 25px;
}

.card {
    background: white;
    border: 1px solid var(--borda);
    border-radius: 20px;
    padding: 28px;
    box-shadow: var(--sombra);
}

.card h3 {
    margin-bottom: 9px;
    color: var(--roxo-escuro);
}

.card p {
    color: var(--cinza);
}

.highlight {
    background: var(--roxo);
    color: white;
    border-color: var(--roxo);
}

.highlight h3,
.highlight p {
    color: white;
}


/* =========================
   COMO FUNCIONA
========================= */

.light {
    background: #faf8fd;
}

.steps {
    display: grid;
    grid-template-columns: repeat(4,1fr);
    gap: 15px;
}

.step {
    background: white;
    border: 1px solid var(--borda);
    border-radius: 18px;
    padding: 23px;
    text-align: center;
}

.step-number {
    width: 46px;
    height: 46px;
    margin: 0 auto 15px;
    border-radius: 50%;
    display: grid;
    place-items: center;
    background: var(--lilas-2);
    color: var(--roxo);
    font-weight: 900;
    font-size: 18px;
}

.step h3 {
    font-size: 17px;
    margin-bottom: 8px;
}

.step p {
    font-size: 14px;
    color: var(--cinza);
}


/* =========================
   FONTES
========================= */

.sources {
    display: grid;
    grid-template-columns: repeat(5,1fr);
    gap: 14px;
}

.source {
    min-height: 130px;
    border: 1px solid var(--borda);
    border-radius: 18px;
    display: flex;
    flex-direction: column;
    justify-content: center;
    align-items: center;
    text-align: center;
    padding: 15px;
    background: white;
}

.source strong {
    font-size: 21px;
    color: var(--roxo);
}

.source small {
    color: var(--cinza);
    margin-top: 5px;
}


/* =========================
   COMUNIDADE
========================= */

.community {
    display: grid;
    grid-template-columns: .9fr 1.1fr;
    gap: 30px;
    align-items: center;
}

.community-box {
    background: linear-gradient(
        135deg,
        var(--roxo),
        #8b4bd1
    );

    color: white;
    border-radius: 26px;
    padding: 35px;
}

.community-box h2 {
    font-size: 34px;
    line-height: 1.1;
    margin-bottom: 13px;
}

.community-box p {
    opacity: .9;
}

.questions {
    display: grid;
    gap: 13px;
}

.question {
    padding: 16px 18px;
    border: 1px solid var(--borda);
    border-radius: 14px;
    background: white;
    font-weight: 700;
}

.question::before {
    content: "✓";
    color: var(--roxo);
    margin-right: 10px;
}


/* =========================
   IMPACTO
========================= */

.benefits {
    display: grid;
    grid-template-columns: repeat(3,1fr);
    gap: 18px;
}

.benefit {
    padding: 25px;
    border: 1px solid var(--borda);
    border-radius: 18px;
}

.benefit .big {
    font-size: 30px;
    color: var(--roxo);
    font-weight: 900;
}

.benefit h3 {
    margin: 8px 0;
}

.benefit p {
    color: var(--cinza);
    font-size: 14px;
}


/* =========================
   FINAL
========================= */

.cta {
    background: var(--roxo-escuro);
    color: white;
    text-align: center;
    padding: 65px 20px;
}

.cta h2 {
    font-size: 40px;
    line-height: 1.1;
    margin-bottom: 13px;
}

.cta p {
    max-width: 680px;
    margin: 0 auto 25px;
    opacity: .88;
}

.cta .btn {
    background: white;
    color: var(--roxo-escuro);
    box-shadow: none;
}


/* =========================
   RODAPÉ
========================= */

footer {
    background: #24113c;
    color: #d9ccea;
    padding: 35px 0;
}

.footer-grid {
    display: flex;
    justify-content: space-between;
    gap: 30px;
    align-items: center;
}

footer strong {
    color: white;
}

footer p {
    font-size: 13px;
}

.team {
    text-align: right;
}


/* =========================
   CELULAR
========================= */

@media(max-width:850px) {

    .nav-links {
        display: none;
    }

    .menu {
        display: block;
    }

    .hero-grid,
    .problem,
    .community {
        grid-template-columns: 1fr;
    }

    .steps {
        grid-template-columns: 1fr 1fr;
    }

    .sources {
        grid-template-columns: 1fr 1fr;
    }

    .benefits {
        grid-template-columns: 1fr;
    }

    .team {
        text-align: left;
    }

    .footer-grid {
        flex-direction: column;
        align-items: flex-start;
    }
}

@media(max-width:520px) {

    .hero {
        padding: 60px 0;
    }

    section {
        padding: 58px 0;
    }

    .steps,
    .sources {
        grid-template-columns: 1fr;
    }

    h1 {
        font-size: 46px;
    }

    .hero p {
        font-size: 17px;
    }
}

</style>
</head>


<body>


<!-- =========================
     MENU
========================= -->

<nav>

<div class="container nav-inner">

<a class="logo" href="#inicio">

<span class="logo-mark">
M
</span>

<span>
MOC
</span>

</a>


<div class="nav-links">

<a href="#problema">
Problema
</a>

<a href="#funciona">
Como funciona
</a>

<a href="#dados">
Dados
</a>

<a href="#comunidade">
Comunidade
</a>

<a href="#impacto">
Impacto
</a>

</div>


<button
class="menu"
aria-label="Abrir menu"
onclick="toggleMenu()">

☰

</button>

</div>

</nav>



<main>


<!-- =========================
     CAPA
========================= -->

<section
class="hero"
id="inicio">

<div class="container hero-grid">


<div>

<span class="badge">
EQUIPE DECODERS • DESAFIO DOS DADOS 2026
</span>


<h1>

Mapa de

<span class="gradient">
Oportunidades
</span>

Culturais

</h1>


<p>

O MOC utiliza Ciência de Dados para identificar
regiões com menor oferta cultural e encontrar
oportunidades para novas atividades e projetos.

</p>


<a
class="btn"
href="#funciona">

Conheça o projeto ↓

</a>

</div>



<div class="hero-card">

<h3>
Da informação à oportunidade
</h3>


<div class="flow">


<div class="flow-item">

<span class="icon">
1
</span>

Coleta de dados

</div>


<div class="flow-item">

<span class="icon">
2
</span>

Tratamento e análise

</div>


<div class="flow-item">

<span class="icon">
3
</span>

Geração de informações

</div>


<div class="flow-item">

<span class="icon">
4
</span>

Identificação de oportunidades

</div>


</div>

</div>

</div>

</section>



<!-- =========================
     PROBLEMA
========================= -->

<section id="problema">

<div class="container">


<div class="section-title">

<span>
O desafio
</span>


<h2>
Por que o MOC existe?
</h2>


<p>

Muitas atividades culturais existem, mas nem sempre
chegam ao conhecimento da população ou são
distribuídas de forma equilibrada pelo município.

</p>

</div>



<div class="problem">


<div class="card">

<h3>
O problema
</h3>


<p>

Pessoas podem ter dificuldade para encontrar
atividades culturais na região onde moram.
Também pode ser difícil identificar quais áreas
precisam de mais ações culturais.

</p>

</div>



<div class="card highlight">

<h3>
A oportunidade
</h3>


<p>

Reunir dados públicos e informações da comunidade
para compreender melhor a realidade cultural e
apontar regiões onde novos projetos podem fazer diferença.

</p>

</div>


</div>

</div>

</section>



<!-- =========================
     COMO FUNCIONA
========================= -->

<section
class="light"
id="funciona">

<div class="container">


<div class="section-title">

<span>
Metodologia
</span>


<h2>
Como funciona?
</h2>


<p>

O projeto transforma diferentes informações em
dados úteis para o planejamento cultural.

</p>

</div>



<div class="steps">


<div class="step">

<div class="step-number">
1
</div>

<h3>
Coleta
</h3>

<p>

Reunimos dados públicos e informações obtidas
por questionários da comunidade.

</p>

</div>



<div class="step">

<div class="step-number">
2
</div>

<h3>
Análise
</h3>

<p>

Os dados são organizados e analisados
utilizando Python.

</p>

</div>



<div class="step">

<div class="step-number">
3
</div>

<h3>
Visualização
</h3>

<p>

Os resultados podem ser apresentados em
gráficos, tabelas e mapas.

</p>

</div>



<div class="step">

<div class="step-number">
4
</div>

<h3>
Oportunidades
</h3>

<p>

As informações ajudam a identificar regiões
que podem receber novas ações culturais.

</p>

</div>


</div>

</div>

</section>



<!-- =========================
     FONTES
========================= -->

<section id="dados">

<div class="container">


<div class="section-title">

<span>
Fontes
</span>


<h2>
De onde vêm os dados?
</h2>


<p>

O projeto utiliza diferentes bases públicas
relacionadas à cultura e à realidade social.

</p>

</div>



<div class="sources">


<div class="source">

<strong>
IBGE
</strong>

<small>
Dados demográficos e indicadores culturais
</small>

</div>



<div class="source">

<strong>
SIIC
</strong>

<small>
Informações sobre cultura e equipamentos culturais
</small>

</div>



<div class="source">

<strong>
Mapa da Cultura
</strong>

<small>
Espaços e atividades culturais
</small>

</div>



<div class="source">

<strong>
TIC Cultura
</strong>

<small>
Acesso à tecnologia e hábitos culturais
</small>

</div>



<div class="source">

<strong>
DataViva
</strong>

<small>
Indicadores socioeconômicos complementares
</small>

</div>


</div>

</div>

</section>



<!-- =========================
     COMUNIDADE
========================= -->

<section
class="light"
id="comunidade">

<div class="container community">


<div class="community-box">

<h2>
A comunidade também participa.
</h2>


<p>

A população pode contribuir por meio de
questionários, ajudando a identificar interesses
culturais, dificuldades de acesso e regiões
que precisam de maior atenção.

</p>

</div>



<div>


<div
class="section-title"
style="text-align:left;margin:0 0 22px">

<span>
Participação
</span>


<h2>
O que queremos descobrir?
</h2>

</div>



<div class="questions">


<div class="question">

Quais atividades culturais a população gostaria
de encontrar?

</div>


<div class="question">

Quais dificuldades existem para participar
dessas atividades?

</div>


<div class="question">

Quais regiões precisam de maior atenção?

</div>


<div class="question">

Como os dados podem apoiar novas ações culturais?

</div>


</div>

</div>

</div>

</section>



<!-- =========================
     IMPACTO
========================= -->

<section id="impacto">

<div class="container">


<div class="section-title">

<span>
Resultados esperados
</span>


<h2>
Que impacto queremos gerar?
</h2>


<p>

O MOC busca aproximar pessoas da cultura
e apoiar decisões baseadas em informações.

</p>

</div>



<div class="benefits">


<div class="benefit">

<div class="big">
01
</div>

<h3>
Mais acesso à cultura
</h3>

<p>

Facilitar a visualização das oportunidades
culturais existentes no município.

</p>

</div>



<div class="benefit">

<div class="big">
02
</div>

<h3>
Mais visibilidade
</h3>

<p>

Valorizar artistas, espaços culturais e
manifestações que podem passar despercebidos.

</p>

</div>



<div class="benefit">

<div class="big">
03
</div>

<h3>
Novos projetos
</h3>

<p>

Apontar regiões com oportunidades para
ampliar a oferta de atividades culturais.

</p>

</div>


</div>

</div>

</section>



<!-- =========================
     FINAL
========================= -->

<section class="cta">

<h2>

Dados que aproximam
<br>

pessoas da cultura.

</h2>


<p>

O MOC mostra como a Ciência de Dados pode
ser utilizada para compreender problemas reais
e apoiar soluções que beneficiem a comunidade.

</p>


<a
class="btn"
href="#inicio">

Voltar ao início ↑

</a>

</section>


</main>



<!-- =========================
     RODAPÉ
========================= -->

<footer>

<div class="container footer-grid">


<div>

<strong>
MOC — Mapa de Oportunidades Culturais
</strong>

<p>
Desafio dos Dados 2026
</p>

</div>



<div class="team">

<strong>
Equipe Decoders
</strong>

<p>
Gabriela • Julia • Kamilla • Vitoria
</p>

</div>


</div>

</footer>



<!-- =========================
     JAVASCRIPT
========================= -->

<script>

function toggleMenu() {

    const links =
        document.querySelector('.nav-links');

    const aberto =
        links.style.display === 'flex';


    links.style.display =
        aberto ? 'none' : 'flex';


    if (!aberto) {

        links.style.position = 'absolute';

        links.style.top = '70px';

        links.style.left = '0';

        links.style.right = '0';

        links.style.background = '#fff';

        links.style.padding = '20px';

        links.style.flexDirection = 'column';

        links.style.borderBottom =
            '1px solid #e3d8ef';

    }

}

</script>


</body>
</html>
