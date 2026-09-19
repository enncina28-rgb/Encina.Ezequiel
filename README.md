# Tema: "Impacto de las modificaciones al régimen de Draw Back y Reintegros a las Exportaciones en las economías regionales de Misiones (2019-2024)"
Por qué este tema:
Es específico a tu carrera y aprovechás lo que ya venís viendo (normativa aduanera, Decreto 1330/2004, regímenes de importación temporaria).
Misiones tiene rubros bien identificables para analizar: yerba mate, té, madera/celulosa, tabaco — todos con expo relevante y sensibles a reintegros.
Hay 5 años (2019-2024) con cambios normativos concretos y visibles: suspensiones/restituciones de reintegros, ajustes por la crisis del dólar, 
retenciones cruzadas, etc. Buen material para el Word.

conectado_con_Netlify
[[sitio-netlify](<!DOCTYPE html>
<html lang="es">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0">
<title>Draw Back &amp; Reintegros — Complejo Yerbatero de Misiones (2019-2024)</title>
<script src="https://cdnjs.cloudflare.com/ajax/libs/Chart.js/4.4.4/chart.umd.min.js"></script>
<style>
  :root{
    --green-900:#12332a;
    --green-800:#1f4e37;
    --green-700:#2e7d4f;
    --green-500:#3f9d64;
    --green-100:#eaf4ec;
    --gold:#c9a24b;
    --cream:#faf7f0;
    --ink:#1c2420;
    --grey:#5c6b63;
    --card:#ffffff;
    --radius:16px;
  }
  :root:not([data-theme="light"]){
    --card:#ffffff;
  }
  @media (prefers-color-scheme: dark){
    :root:not([data-theme="light"]){
      --cream:#0f1512;
      --ink:#eef2ef;
      --grey:#a9b6ae;
      --card:#182420;
      --green-100:#16261f;
    }
  }
  :root[data-theme="dark"]{
    --cream:#0f1512;
    --ink:#eef2ef;
    --grey:#a9b6ae;
    --card:#182420;
    --green-100:#16261f;
  }
  *{box-sizing:border-box;}
  body{
    margin:0;
    font-family:'Georgia', 'Times New Roman', serif;
    background:var(--cream);
    color:var(--ink);
    line-height:1.6;
  }
  .sans{font-family:Arial, Helvetica, sans-serif;}
  header.hero{
    background:linear-gradient(135deg, var(--green-900), var(--green-700));
    color:#fff;
    padding:72px 24px 96px;
    position:relative;
    overflow:hidden;
  }
  header.hero .wrap{max-width:980px;margin:0 auto;position:relative;z-index:2;}
  header.hero .kicker{
    font-family:Arial, sans-serif;
    letter-spacing:.14em;
    text-transform:uppercase;
    font-size:12px;
    color:var(--gold);
    margin-bottom:14px;
  }
  header.hero h1{
    font-size:clamp(28px, 4.4vw, 46px);
    margin:0 0 16px;
    line-height:1.15;
  }
  header.hero p.lead{
    font-family:Arial, sans-serif;
    font-size:17px;
    max-width:640px;
    color:#e4efe8;
  }
  .leaf-deco{
    position:absolute; right:-60px; top:-40px; opacity:.18;
    width:340px; height:340px;
  }
  main{max-width:980px;margin:-56px auto 0;padding:0 24px 80px;position:relative;z-index:3;}
  .card{
    background:var(--card);
    border-radius:var(--radius);
    box-shadow:0 10px 30px rgba(18,51,42,.10);
    padding:36px 32px;
    margin-bottom:28px;
  }
  .card h2{
    font-family:Arial, sans-serif;
    color:var(--green-800);
    font-size:24px;
    margin-top:0;
    display:flex;align-items:center;gap:10px;
  }
  .card h2 .num{
    background:var(--green-700);color:#fff;border-radius:50%;
    width:32px;height:32px;display:inline-flex;align-items:center;justify-content:center;
    font-size:15px;flex:none;
  }
  .card h3{
    font-family:Arial, sans-serif;
    color:var(--green-700);
    font-size:17px;
    margin:22px 0 8px;
  }
  p{margin:0 0 14px;}
  .grid2{display:grid;grid-template-columns:1fr 1fr;gap:24px;}
  @media (max-width:720px){.grid2{grid-template-columns:1fr;}}
  .stat{
    background:var(--green-100);
    border-radius:12px;
    padding:18px 20px;
    text-align:center;
    font-family:Arial, sans-serif;
  }
  .stat .big{font-size:28px;font-weight:bold;color:var(--green-800);}
  .stat .label{font-size:12.5px;color:var(--grey);margin-top:4px;}
  .stats-row{display:flex;gap:16px;flex-wrap:wrap;margin:20px 0;}
  .stats-row .stat{flex:1;min-width:130px;}
  table{width:100%;border-collapse:collapse;font-family:Arial, sans-serif;font-size:14px;margin:12px 0 6px;}
  th{
    background:var(--green-700);color:#fff;text-align:left;padding:10px 12px;
    font-size:13px;
  }
  td{padding:10px 12px;border-bottom:1px solid rgba(0,0,0,.08);vertical-align:top;}
  tr:nth-child(even) td{background:rgba(46,125,79,.05);}
  .badge{
    display:inline-block;font-family:Arial,sans-serif;font-size:11.5px;
    padding:3px 10px;border-radius:999px;background:var(--gold);color:#3a2c05;font-weight:bold;
  }
  .badge.exp{background:#dcefe1;color:var(--green-800);}
  .badge.mix{background:#f5e6c8;color:#6b4f11;}
  .badge.res{background:#f1d9d9;color:#7a2d2d;}
  canvas{max-width:100%;}
  ul.clean{margin:0 0 10px;padding-left:20px;}
  ul.clean li{margin-bottom:8px;}
  footer{
    text-align:center;font-family:Arial, sans-serif;font-size:12.5px;color:var(--grey);
    padding:20px 24px 50px;
  }
  .source-note{
    font-family:Arial, sans-serif;font-size:11.5px;color:var(--grey);font-style:italic;
    border-top:1px dashed rgba(0,0,0,.15);padding-top:10px;margin-top:14px;
  }
  .illus{width:100%;max-width:420px;display:block;margin:0 auto;}
  .toc{font-family:Arial, sans-serif;font-size:14px;}
  .toc a{color:var(--green-700);text-decoration:none;}
  .toc a:hover{text-decoration:underline;}
  .toc ol{padding-left:20px;}
  .toc li{margin-bottom:6px;}
</style>
</head>
<body>

<header class="hero">
  <svg class="leaf-deco" viewBox="0 0 200 200" xmlns="http://www.w3.org/2000/svg">
    <path d="M100 10 C 40 40, 20 110, 100 190 C 180 110, 160 40, 100 10 Z" fill="#ffffff"/>
    <path d="M100 20 L100 180" stroke="#1f4e37" stroke-width="4"/>
  </svg>
  <div class="wrap">
    <div class="kicker sans">Comercio Internacional y Despacho Aduanero · Instituto Alfa</div>
    <h1>Draw Back y Reintegros a la Exportación:<br>impacto en el Complejo Yerbatero de Misiones</h1>
    <p class="lead">Análisis estadístico de exportaciones (2019-2024) cruzado con las modificaciones normativas de Derechos de Exportación y Reintegros en Argentina.</p>
  </div>
</header>

<main>

  <section class="card toc">
    <h2 class="sans"><span class="num">•</span>Índice</h2>
    <ol>
      <li><a href="#contexto">Contexto y objetivo del análisis</a></li>
      <li><a href="#datos">Datos estadísticos de exportación (2019-2024)</a></li>
      <li><a href="#normativa">Cronología normativa: Draw Back y Reintegros</a></li>
      <li><a href="#cruce">Cruce: normativa vs. desempeño exportador</a></li>
      <li><a href="#conclusiones">Conclusiones</a></li>
      <li><a href="#fuentes">Fuentes</a></li>
    </ol>
  </section>

  <section class="card" id="contexto">
    <h2><span class="num">1</span>Contexto y objetivo</h2>
    <p>La yerba mate es uno de los principales productos de la economía regional de Misiones y Corrientes,
    con Argentina como primer productor y segundo exportador mundial. Su comercio exterior está directamente
    influido por los Derechos de Exportación (retenciones) y los Reintegros que el Estado nacional define
    periódicamente mediante decretos y resoluciones.</p>
    <p>Este trabajo integra dos fuentes: <strong>datos estadísticos de exportación</strong> de los últimos
    cinco años y <strong>modificaciones normativas</strong> sobre Draw Back / Reintegros, para evaluar si
    existe una relación entre los incentivos fiscales al exportador y el desempeño real del sector.</p>
    <svg class="illus" viewBox="0 0 420 160" xmlns="http://www.w3.org/2000/svg">
      <rect x="0" y="120" width="420" height="6" fill="#c9a24b" opacity="0.5"/>
      <circle cx="70" cy="90" r="46" fill="#eaf4ec"/>
      <path d="M70 55 C40 70, 30 110, 70 130 C110 110, 100 70, 70 55 Z" fill="#2e7d4f"/>
      <g transform="translate(180,40)">
        <rect x="0" y="70" width="30" height="40" fill="#2e7d4f"/>
        <rect x="40" y="45" width="30" height="65" fill="#3f9d64"/>
        <rect x="80" y="20" width="30" height="90" fill="#1f4e37"/>
        <rect x="120" y="55" width="30" height="55" fill="#c9a24b"/>
      </g>
      <g transform="translate(340,55)">
        <path d="M0 40 Q20 0 60 10 Q55 45 0 40Z" fill="#3f9d64"/>
      </g>
    </svg>
  </section>

  <section class="card" id="datos">
    <h2><span class="num">2</span>Datos estadísticos de exportación (2019-2024)</h2>
    <p>Volumen exportado de yerba mate y derivados, según INYM/INDEC. Ver detalle completo, con fórmulas
    y variación interanual, en el archivo <em>Excel 1</em> adjunto.</p>

    <div class="stats-row">
      <div class="stat"><div class="big">44.019 Tn</div><div class="label">Récord exportado en 2024</div></div>
      <div class="stat"><div class="big">+10,7%</div><div class="label">Crecimiento acumulado 2019-2024</div></div>
      <div class="stat"><div class="big">~70%</div><div class="label">Participación de Siria (2024)</div></div>
    </div>

    <canvas id="volChart" height="120"></canvas>
    <canvas id="valChart" height="120" style="margin-top:30px;"></canvas>
    <p class="source-note">Fuente: INYM, INDEC y Bolsa de Comercio de Rosario. Precio FOB promedio estimado
    en base a informes sectoriales (CAME/BCR) — ver Excel 1 para el detalle año a año.</p>
  </section>

  <section class="card" id="normativa">
    <h2><span class="num">3</span>Cronología normativa: Draw Back y Reintegros</h2>
    <p>Principales decretos y resoluciones que modificaron Derechos de Exportación, Reintegros y el
    marco cambiario para exportadores de economías regionales entre 2019 y 2024 (desarrollo completo en
    el documento Word adjunto).</p>
    <table>
      <thead><tr><th>Año</th><th>Norma</th><th>Tipo</th></tr></thead>
      <tbody>
        <tr><td>2019</td><td>Decreto 37/2019</td><td><span class="badge res">Restrictiva</span></td></tr>
        <tr><td>2020</td><td>Decretos 1060/2020 y 789/2020</td><td><span class="badge exp">Expansiva</span></td></tr>
        <tr><td>2021</td><td>Decreto 410/2021</td><td><span class="badge exp">Expansiva</span></td></tr>
        <tr><td>2022</td><td>Decretos 576/2022 y 787/2022</td><td><span class="badge exp">Expansiva</span></td></tr>
        <tr><td>2023</td><td>Decreto 194/2023, Res. 138/2023, DNU 70/2023</td><td><span class="badge mix">Mixta</span></td></tr>
        <tr><td>2024</td><td>RG AFIP 5551/2024 y 5553/2024</td><td><span class="badge exp">Expansiva (administrativa)</span></td></tr>
      </tbody>
    </table>
  </section>

  <section class="card" id="cruce">
    <h2><span class="num">4</span>Cruce: normativa vs. desempeño exportador</h2>
    <canvas id="crossChart" height="130"></canvas>
    <h3>Lectura del cruce</h3>
    <ul class="clean">
      <li><strong>2020-2021:</strong> pese a medidas expansivas (Decretos 1060/789 de 2020 y 410/2021),
      el volumen exportado cayó en 2021, explicado por factores climáticos y de demanda externa ajenos a
      la política arancelaria.</li>
      <li><strong>2022-2023:</strong> los programas de incentivo cambiario ("dólar soja/agro") coincidieron
      con una recuperación y luego estabilización del volumen exportado.</li>
      <li><strong>2024:</strong> la simplificación administrativa y la mayor demanda de Siria impulsaron un
      récord histórico de exportaciones.</li>
    </ul>
  </section>

  <section class="card" id="conclusiones">
    <h2><span class="num">5</span>Conclusiones</h2>
    <ul class="clean">
      <li>El período 2019-2024 muestra una tendencia de fondo hacia la reducción de Derechos de Exportación
      y la ampliación de reintegros para economías regionales.</li>
      <li>Los incentivos cambiarios de 2022-2023 funcionaron como mecanismo complementario a los reintegros
      tradicionales para sostener la competitividad exportadora.</li>
      <li>La relación entre normativa favorable y volumen exportado no es lineal: otros factores (clima,
      demanda internacional, tipo de cambio real) inciden con igual o mayor peso.</li>
      <li>El cierre del período combina desregulación sectorial (fin de precios mínimos del INYM) y
      simplificación administrativa, anticipando la profundización de ese rumbo en 2025.</li>
    </ul>
  </section>

  <section class="card" id="fuentes">
    <h2><span class="num">6</span>Fuentes</h2>
    <p class="source-note" style="border:none;padding:0;">
      Boletín Oficial de la República Argentina · Instituto Nacional de la Yerba Mate (INYM) · INDEC ·
      Bolsa de Comercio de Rosario (BCR) · Centro de Economía Política (CEPA) · KPMG Argentina (Novedades Tax) ·
      Ministerio de Agricultura, Ganadería y Pesca (magyp.gob.ar) · El Economista · Infocampo · Bichos de Campo.
      Elaboración propia a partir de normativa pública e informes sectoriales, como trabajo práctico de
      Comercio Internacional y Despacho Aduanero.
    </p>
  </section>

</main>

<footer>
  Instituto Alfa — Comercio Internacional y Despacho Aduanero · Posadas, Misiones, Argentina
</footer>

<script>
const yearLabels = ['2019','2020','2021','2022','2023','2024'];
const volumen = [39800, 42906, 35510, 40304, 39701, 44019];
const valorFOB = volumen.map((v,i)=> v * [1850,1900,2010,2170,2245,2050][i]);

function baseOptions(titleText, yLabel){
  return {
    responsive:true,
    plugins:{
      legend:{display:false},
      title:{display:true, text:titleText, font:{size:15, family:'Arial'}, color:'#1f4e37'}
    },
    scales:{
      y:{title:{display:true,text:yLabel,font:{family:'Arial'}}, grid:{color:'rgba(0,0,0,.06)'}},
      x:{grid:{display:false}}
    }
  };
}

new Chart(document.getElementById('volChart'), {
  type:'bar',
  data:{labels:yearLabels, datasets:[{label:'Volumen (Tn)', data:volumen, backgroundColor:'#2e7d4f', borderRadius:6}]},
  options: baseOptions('Volumen exportado de yerba mate (Tn)', 'Toneladas')
});

new Chart(document.getElementById('valChart'), {
  type:'line',
  data:{labels:yearLabels, datasets:[{label:'Valor FOB (USD)', data:valorFOB, borderColor:'#c9a24b', backgroundColor:'rgba(201,162,75,.25)', fill:true, tension:.3, pointBackgroundColor:'#c9a24b'}]},
  options: baseOptions('Valor FOB exportado estimado (USD)', 'USD')
});

new Chart(document.getElementById('crossChart'), {
  type:'bar',
  data:{
    labels:yearLabels,
    datasets:[
      {label:'Volumen (Tn)', data:volumen, backgroundColor:'#2e7d4f', borderRadius:6, order:2},
    ]
  },
  options: {
    responsive:true,
    plugins:{
      legend:{display:false},
      title:{display:true, text:'Volumen exportado y principales hitos normativos', font:{size:15, family:'Arial'}, color:'#1f4e37'},
      subtitle:{display:true, text:'2019: Dto.37 · 2020: Dtos.1060/789 · 2021: Dto.410 · 2022: Dtos.576/787 · 2023: Dto.194/DNU70 · 2024: RG AFIP', font:{size:11, family:'Arial'}, color:'#5c6b63'}
    },
    scales:{ y:{title:{display:true,text:'Toneladas',font:{family:'Arial'}}}, x:{grid:{display:false}} }
  }
});
</script>

</body>
</html>)]
