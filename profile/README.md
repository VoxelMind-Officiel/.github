<!doctype html>
<html lang="fr">
<head>
  <meta charset="utf-8" />
  <meta name="viewport" content="width=device-width,initial-scale=1" />
  <title>VoxelMind — Présentation</title>
  <style>
    :root{
      --bg:#0f1724; --card:#0b1220; --accent:#6ee7b7; --muted:#9ba6b2; --glass: rgba(255,255,255,0.04);
      --radius:16px; --pad:24px; font-family:Inter, system-ui, -apple-system, 'Segoe UI', Roboto, 'Helvetica Neue', Arial;
    }
    *{box-sizing:border-box}
    body{margin:0;background:linear-gradient(180deg,#071028 0%, #081426 60%);color:#e6eef6;-webkit-font-smoothing:antialiased}
    .container{max-width:1100px;margin:40px auto;padding:20px}
    header{display:flex;align-items:center;gap:18px}
    .logo{width:72px;height:72px;border-radius:14px;background:linear-gradient(135deg,var(--accent),#7dd3fc);display:flex;align-items:center;justify-content:center;color:#062024;font-weight:800;font-size:20px;box-shadow:0 6px 24px rgba(0,0,0,0.5)}
    h1{margin:0;font-size:28px}
    p.lead{color:var(--muted);margin-top:6px}

    .hero{display:grid;grid-template-columns:1fr 420px;gap:28px;margin-top:28px}
    .card{background:linear-gradient(180deg,var(--card), rgba(255,255,255,0.02));border-radius:var(--radius);padding:var(--pad);box-shadow:0 8px 30px rgba(2,6,23,0.6)}
    .buttons{display:flex;gap:12px;margin-top:16px}
    .btn{padding:10px 14px;border-radius:10px;background:var(--glass);border:1px solid rgba(255,255,255,0.04);cursor:pointer}
    .btn.primary{background:linear-gradient(90deg,var(--accent),#7dd3fc);color:#062024;font-weight:700}

    /* preview phone mock */
    .mock{height:560px;border-radius:18px;overflow:hidden;border:1px solid rgba(255,255,255,0.04);display:flex;flex-direction:column}
    .mock .top{height:56px;background:linear-gradient(90deg,#062b37, #072a4a);display:flex;align-items:center;padding:12px 16px;color:var(--accent);font-weight:700}
    .mock .screen{flex:1;padding:18px;background:linear-gradient(180deg, rgba(255,255,255,0.012), transparent)}
    .screenshot{height:100%;border-radius:10px;background:linear-gradient(180deg,#071128, #09203a);display:flex;flex-direction:column}
    .screenshot h3{margin:18px 18px 8px;font-size:16px}
    .screenshot p{margin:0 18px;color:var(--muted);font-size:13px}

    /* Projects */
    .grid{display:grid;grid-template-columns:repeat(2,1fr);gap:18px;margin-top:20px}
    .project-badge{display:inline-block;padding:6px 10px;border-radius:999px;background:rgba(255,255,255,0.03);border:1px solid rgba(255,255,255,0.02);font-weight:600}
    .project-list .project{display:flex;gap:12px;align-items:flex-start}
    .thumb{width:88px;height:64px;border-radius:10px;background:linear-gradient(135deg,#0b3b2f,#063064);display:flex;align-items:center;justify-content:center;font-weight:700}

    footer{margin-top:36px;color:var(--muted);font-size:13px;padding:12px 0}

    @media(max-width:900px){.hero{grid-template-columns:1fr;}.grid{grid-template-columns:1fr}}
  </style>
</head>
<body>
  <div class="container">
    <header>
      <div class="logo">VM</div>
      <div>
        <h1>VoxelMind — Studio & Communauté</h1>
        <p class="lead">Nous créons des expériences Minecraft originales et des outils pour la communauté. Voici un aperçu de VoxelMind et de nos projets en cours.</p>
      </div>
    </header>

    <section class="hero">
      <div class="card">
        <div style="display:flex;justify-content:space-between;align-items:start;gap:12px">
          <div>
            <span class="project-badge">Équipe</span>
            <h2 style="margin:10px 0 4px">À propos de VoxelMind</h2>
            <p style="color:var(--muted);margin:0 0 12px">VoxelMind est un collectif de développeurs, moddeurs et créateurs qui développent des mods, serveurs et expériences narratifs pour Minecraft.</p>
          </div>
          <div style="text-align:right">
            <div style="font-weight:700">Status</div>
            <div style="color:var(--accent);font-weight:800;margin-top:6px">Actif — Recrutement ouvert</div>
          </div>
        </div>

        <div style="margin-top:16px">
          <h3 style="margin:0 0 8px">Projets</h3>
          <div class="project-list">
            <div class="project card" style="margin-bottom:10px;padding:12px;display:flex;align-items:center">
              <div class="thumb">EQ</div>
              <div style="flex:1">
                <strong>EarthQuest</strong>
                <div style="color:var(--muted);font-size:13px">Un projet d'aventure/éducation sur Minecraft visant à recréer des biomes, quêtes et mécaniques autour de l'écologie et de la coopération.</div>
              </div>
              <div style="text-align:right;color:var(--muted);font-size:13px">Version cible: 1.7.10 (bibliothèques compatibles)</div>
            </div>

            <!-- autre projets à venir -->
            <div class="project card" style="padding:12px;opacity:0.6">
              <div class="thumb" style="background:linear-gradient(135deg,#2b2f4a,#1b2540)">+</div>
              <div style="flex:1">
                <strong>Bientôt</strong>
                <div style="color:var(--muted);font-size:13px">Nouveaux modules, mods et outils — détails à venir.</div>
              </div>
              <div style="text-align:right;color:var(--muted);font-size:13px">Backlog</div>
            </div>
          </div>
        </div>

        <div style="margin-top:14px;display:flex;gap:10px">
          <div class="btn primary">Voir sur GitHub</div>
          <div class="btn">Se joindre au Discord</div>
        </div>

        <div style="margin-top:18px;color:var(--muted);font-size:13px">
          <strong>Contribuer</strong>
          <div>Issues, PRs, tests et idées — bienvenue. Nous utilisons GitHub pour le code et Discord pour la coordination.</div>
        </div>
      </div>

      <aside class="mock card" aria-hidden="true">
        <div class="top">VoxelMind — Aperçu</div>
        <div class="screen">
          <div class="screenshot">
            <h3>EarthQuest — Page du projet</h3>
            <p>Explorez, restaurez et apprenez : mécaniques de quêtes, inventaire personnalisé, et intégration éducative.</p>
            <div style="margin:12px 18px 0;display:flex;gap:8px;flex-wrap:wrap">
              <span style="padding:6px 8px;border-radius:8px;background:rgba(255,255,255,0.02);font-size:12px">Quêtes</span>
              <span style="padding:6px 8px;border-radius:8px;background:rgba(255,255,255,0.02);font-size:12px">Biomes personnalisés</span>
              <span style="padding:6px 8px;border-radius:8px;background:rgba(255,255,255,0.02);font-size:12px">Éducation</span>
            </div>
            <div style="margin-top:auto;padding:18px">
              <div style="display:flex;gap:8px;align-items:center">
                <div style="width:44px;height:44px;border-radius:8px;background:linear-gradient(135deg,#8ef6c2,#7dd3fc);display:flex;align-items:center;justify-content:center;font-weight:800;color:#062024">EQ</div>
                <div>
                  <div style="font-weight:700">EarthQuest</div>
                  <div style="color:var(--muted);font-size:12px">Prototype jouable — mécaniques, quêtes et assets.</div>
                </div>
                <div style="margin-left:auto;color:var(--muted);font-size:12px">Dernière mise à jour: Avril 2025</div>
              </div>
            </div>
          </div>
        </div>
      </aside>
    </section>

    <section style="margin-top:22px" class="card">
      <h3 style="margin-top:0">Stack & outils</h3>
      <p style="color:var(--muted);margin:6px 0 12px">Java, Forge, Jsoup, AdonisJS (services web), React (UI externes), et outils d'intégration CI basiques.</p>
      <div style="display:flex;gap:12px;flex-wrap:wrap">
        <div class="btn">Java / Forge</div>
        <div class="btn">Jsoup</div>
        <div class="btn">AdonisJS</div>
        <div class="btn">React</div>
        <div class="btn">GitHub</div>
      </div>
    </section>

    <footer>
      <div style="display:flex;justify-content:space-between;align-items:center;gap:12px">
        <div>© VoxelMind — Créé par l'équipe. Contact: contact@voxelmind.example</div>
        <div style="color:var(--muted)">Voir le README détaillé et les assets dans le repo.</div>
      </div>
    </footer>
  </div>
</body>
</html>
