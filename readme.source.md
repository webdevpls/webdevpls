```aura width=800 height=380
<div style={{ position: 'relative', display: 'flex', flexDirection: 'column', alignItems: 'center', justifyContent: 'center', width: '100%', height: '100%', background: '#08080d', borderRadius: 20, overflow: 'hidden', fontFamily: 'Inter, sans-serif' }}>
  <style>{`
    @keyframes orb-a { 0%, 100% { transform: translate(0, 0); opacity: 0.6; } 50% { transform: translate(28px, -22px); opacity: 0.9; } }
    @keyframes orb-b { 0%, 100% { transform: translate(0, 0); opacity: 0.5; } 50% { transform: translate(-22px, 18px); opacity: 0.75; } }
    @keyframes orb-c { 0%, 100% { transform: translate(0, 0); opacity: 0.35; } 50% { transform: translate(16px, -28px); opacity: 0.6; } }
    @keyframes ring-blink { 0%, 100% { opacity: 0.06; } 50% { opacity: 0.18; } }
    @keyframes ring-blink-b { 0%, 100% { opacity: 0.04; } 50% { opacity: 0.12; } }
    @keyframes dot-spin { 0% { transform: rotate(0deg); } 100% { transform: rotate(360deg); } }
    #hero-o1 { animation: orb-a 9s ease-in-out infinite; }
    #hero-o2 { animation: orb-b 11s ease-in-out infinite 0.8s; }
    #hero-o3 { animation: orb-a 8s ease-in-out infinite 2s; }
    #hero-o4 { animation: orb-b 13s ease-in-out infinite 0.4s; }
    #hero-o5 { animation: orb-c 7s ease-in-out infinite 1.2s; }
    #hr1 { animation: ring-blink 8s ease-in-out infinite; }
    #hr2 { animation: ring-blink 8s ease-in-out infinite 1.4s; }
    #hr3 { animation: ring-blink-b 8s ease-in-out infinite 2.8s; }
    #hr4 { animation: ring-blink-b 8s ease-in-out infinite 4.2s; }
    #hr5 { animation: ring-blink-b 10s ease-in-out infinite 5.6s; }
    #hero-dot { animation: dot-spin 20s linear infinite; }
  `}</style>

  <svg width="800" height="380" style={{ position: 'absolute', top: 0, left: 0 }}>
    <defs>
      <radialGradient id="hg1" cx="50%" cy="50%" r="50%">
        <stop offset="0%" stopColor="rgba(108,195,130,0.55)" />
        <stop offset="100%" stopColor="rgba(108,195,130,0)" />
      </radialGradient>
      <radialGradient id="hg2" cx="50%" cy="50%" r="50%">
        <stop offset="0%" stopColor="rgba(230,100,115,0.5)" />
        <stop offset="100%" stopColor="rgba(230,100,115,0)" />
      </radialGradient>
      <radialGradient id="hg3" cx="50%" cy="50%" r="50%">
        <stop offset="0%" stopColor="rgba(195,155,255,0.35)" />
        <stop offset="100%" stopColor="rgba(195,155,255,0)" />
      </radialGradient>
      <radialGradient id="hg4" cx="50%" cy="50%" r="50%">
        <stop offset="0%" stopColor="rgba(255,195,110,0.28)" />
        <stop offset="100%" stopColor="rgba(255,195,110,0)" />
      </radialGradient>
      <radialGradient id="hg5" cx="50%" cy="50%" r="50%">
        <stop offset="0%" stopColor="rgba(80,160,220,0.3)" />
        <stop offset="100%" stopColor="rgba(80,160,220,0)" />
      </radialGradient>
    </defs>
    <ellipse id="hero-o1" cx="110" cy="310" rx="260" ry="200" fill="url(#hg1)" />
    <ellipse id="hero-o2" cx="710" cy="70" rx="230" ry="190" fill="url(#hg2)" />
    <ellipse id="hero-o3" cx="620" cy="330" rx="200" ry="160" fill="url(#hg3)" />
    <ellipse id="hero-o4" cx="200" cy="55" rx="190" ry="150" fill="url(#hg4)" />
    <ellipse id="hero-o5" cx="400" cy="340" rx="170" ry="130" fill="url(#hg5)" />
    <circle id="hr1" cx="400" cy="178" r="52"  fill="none" stroke="rgba(255,255,255,0.9)" strokeWidth="0.7" />
    <circle id="hr2" cx="400" cy="178" r="92"  fill="none" stroke="rgba(255,255,255,0.9)" strokeWidth="0.7" />
    <circle id="hr3" cx="400" cy="178" r="138" fill="none" stroke="rgba(255,255,255,0.9)" strokeWidth="0.7" />
    <circle id="hr4" cx="400" cy="178" r="192" fill="none" stroke="rgba(255,255,255,0.9)" strokeWidth="0.7" />
    <circle id="hr5" cx="400" cy="178" r="256" fill="none" stroke="rgba(255,255,255,0.9)" strokeWidth="0.7" />
    <g id="hero-dot">
      <circle cx="400" cy="126" r="2.5" fill="rgba(255,255,255,0.5)" />
    </g>
  </svg>

  <div style={{ position: 'relative', display: 'flex', flexDirection: 'column', alignItems: 'center', zIndex: 10 }}>
    <img src={(github && github.user && github.user.avatarUrl) || 'https://avatars.githubusercontent.com/u/89544240?v=4'} width={84} height={84} style={{ borderRadius: 42, border: '2px solid rgba(255,255,255,0.25)', marginBottom: 18 }} />
    <span style={{ fontSize: 60, fontWeight: 700, color: '#ffffff', letterSpacing: -2, lineHeight: 1 }}>Pedro Lucas</span>
    <span style={{ fontSize: 13, color: 'rgba(255,255,255,0.4)', marginTop: 16, letterSpacing: 5, textTransform: 'uppercase', fontWeight: 300 }}>ceo & founder · vision studios</span>
    <div style={{ display: 'flex', gap: 8, marginTop: 30 }}>
      <span style={{ padding: '5px 16px', background: 'rgba(255,255,255,0.04)', color: 'rgba(255,255,255,0.55)', borderRadius: 100, fontSize: 11, border: '1px solid rgba(255,255,255,0.09)', letterSpacing: 1 }}>📍 brasil</span>
      <span style={{ padding: '5px 16px', background: 'rgba(255,255,255,0.04)', color: 'rgba(255,255,255,0.55)', borderRadius: 100, fontSize: 11, border: '1px solid rgba(255,255,255,0.09)', letterSpacing: 1 }}>dev & ui/ux</span>
      <span style={{ padding: '5px 16px', background: 'rgba(255,255,255,0.04)', color: 'rgba(255,255,255,0.55)', borderRadius: 100, fontSize: 11, border: '1px solid rgba(255,255,255,0.09)', letterSpacing: 1 }}>construindo em público</span>
    </div>
  </div>
</div>
```

```aura width=800 height=220
<div style={{ display: 'flex', flexDirection: 'row', gap: 16, width: '100%', height: '100%', fontFamily: 'Inter, sans-serif' }}>
  <style>{`
    @keyframes about-orb-l { 0%, 100% { transform: translate(0,0); opacity: 0.65; } 50% { transform: translate(20px,-14px); opacity: 0.9; } }
    @keyframes about-orb-r { 0%, 100% { transform: translate(0,0); opacity: 0.55; } 50% { transform: translate(-16px,12px); opacity: 0.8; } }
    @keyframes about-ring { 0%, 100% { opacity: 0.07; } 50% { opacity: 0.2; } }
    @keyframes about-ring-b { 0%, 100% { opacity: 0.04; } 50% { opacity: 0.13; } }
    @keyframes cursor-blink { 0%, 100% { opacity: 1; } 49% { opacity: 1; } 50% { opacity: 0; } 99% { opacity: 0; } }
    #ab-o1 { animation: about-orb-l 8s ease-in-out infinite; }
    #ab-o2 { animation: about-orb-r 10s ease-in-out infinite 1s; }
    #ab-o3 { animation: about-orb-l 7s ease-in-out infinite 2s; }
    #ab-r1 { animation: about-ring 7s ease-in-out infinite; }
    #ab-r2 { animation: about-ring 7s ease-in-out infinite 2s; }
    #ab-r3 { animation: about-ring-b 7s ease-in-out infinite 3.5s; }
    #ab-cursor { animation: cursor-blink 1.1s step-end infinite; }
  `}</style>

  <div style={{ position: 'relative', display: 'flex', flex: 1, height: '100%', background: '#08080d', borderRadius: 16, overflow: 'hidden' }}>
    <img src="https://media1.giphy.com/media/v1.Y2lkPTc5MGI3NjExbmVyNmVtYnVubXg1Mmw1MTZ5Y29hdXN0dzJlOTFtNzVmNWwycmgxbyZlcD12MV9pbnRlcm5hbF9naWZfYnlfaWQmY3Q9Zw/fVsVfxVwz40I24GT7X/giphy.gif" style={{ position: 'absolute', top: 0, left: 0, width: '100%', height: '100%', objectFit: 'cover', opacity: 0.35 }} />
    <svg width="100%" height="220" style={{ position: 'absolute', top: 0, left: 0 }}>
      <defs>
        <radialGradient id="ab-gl" cx="50%" cy="50%" r="50%">
          <stop offset="0%" stopColor="rgba(108,195,130,0.6)" />
          <stop offset="100%" stopColor="rgba(108,195,130,0)" />
        </radialGradient>
        <radialGradient id="ab-gr" cx="50%" cy="50%" r="50%">
          <stop offset="0%" stopColor="rgba(230,100,115,0.5)" />
          <stop offset="100%" stopColor="rgba(230,100,115,0)" />
        </radialGradient>
        <radialGradient id="ab-gb" cx="50%" cy="50%" r="50%">
          <stop offset="0%" stopColor="rgba(195,155,255,0.35)" />
          <stop offset="100%" stopColor="rgba(195,155,255,0)" />
        </radialGradient>
      </defs>
      <ellipse id="ab-o1" cx="40"  cy="180" rx="130" ry="110" fill="url(#ab-gl)" />
      <ellipse id="ab-o2" cx="320" cy="40"  rx="120" ry="100" fill="url(#ab-gr)" />
      <ellipse id="ab-o3" cx="260" cy="200" rx="100" ry="90"  fill="url(#ab-gb)" />
      <circle id="ab-r1" cx="165" cy="110" r="38"  fill="none" stroke="rgba(255,255,255,0.9)" strokeWidth="0.7" />
      <circle id="ab-r2" cx="165" cy="110" r="65"  fill="none" stroke="rgba(255,255,255,0.9)" strokeWidth="0.7" />
      <circle id="ab-r3" cx="165" cy="110" r="100" fill="none" stroke="rgba(255,255,255,0.9)" strokeWidth="0.7" />
    </svg>
    <div style={{ position: 'relative', display: 'flex', flexDirection: 'column', justifyContent: 'center', padding: '0 28px', zIndex: 10 }}>
      <span style={{ fontSize: 11, color: 'rgba(255,255,255,0.35)', letterSpacing: 3, textTransform: 'uppercase', marginBottom: 10 }}>sobre mim</span>
      <span style={{ fontSize: 22, fontWeight: 600, color: '#ffffff', lineHeight: 1.3 }}>Trabalho pequeno e útil</span>
      <span style={{ fontSize: 22, fontWeight: 600, color: '#ffffff', lineHeight: 1.3 }}>acima de promessas vagas.</span>
      <div style={{ display: 'flex', alignItems: 'center', marginTop: 14 }}>
        <span style={{ fontSize: 13, color: 'rgba(255,255,255,0.45)', fontFamily: 'monospace' }}>{'> aberto a novos projetos'}</span>
        <span id="ab-cursor" style={{ fontSize: 13, color: 'rgba(255,255,255,0.6)', fontFamily: 'monospace', marginLeft: 1 }}>_</span>
      </div>
    </div>
  </div>

  <div style={{ display: 'flex', flexDirection: 'column', gap: 16, width: 220, flexShrink: 0 }}>
    <div style={{ position: 'relative', display: 'flex', flex: 1, background: '#08080d', borderRadius: 16, overflow: 'hidden', alignItems: 'center', justifyContent: 'center' }}>
      <img src="https://media0.giphy.com/media/v1.Y2lkPTc5MGI3NjExZW95cTRnOXM1dTc1YTFwNjRkcGNkN2RqYjdhdTB3NTc3NDFiNjFxYyZlcD12MV9pbnRlcm5hbF9naWZfYnlfaWQmY3Q9Zw/h58dtf5vTpjulO4M5o/giphy.gif" style={{ position: 'absolute', top: 0, left: 0, width: '100%', height: '100%', objectFit: 'cover', opacity: 0.3 }} />
      <div style={{ position: 'relative', display: 'flex', flexDirection: 'column', alignItems: 'center', zIndex: 10 }}>
        <span style={{ fontSize: 32, fontWeight: 700, color: '#ffffff' }}>🇧🇷</span>
        <span style={{ fontSize: 11, color: 'rgba(255,255,255,0.4)', letterSpacing: 2, textTransform: 'uppercase', marginTop: 4 }}>base no brasil</span>
      </div>
    </div>
    <div style={{ position: 'relative', display: 'flex', flex: 1, background: '#08080d', borderRadius: 16, overflow: 'hidden', alignItems: 'center', justifyContent: 'center' }}>
      <img src="https://media4.giphy.com/media/v1.Y2lkPTc5MGI3NjExemdhbXMwdWNkaDA5eTM4Y3ZjYnYzNTR5YnB0M21jdzlrd2gyczQxNyZlcD12MV9pbnRlcm5hbF9naWZfYnlfaWQmY3Q9Zw/VGh13y4IVFZzCACfTX/giphy.gif" style={{ position: 'absolute', top: 0, left: 0, width: '100%', height: '100%', objectFit: 'cover', opacity: 0.3 }} />
      <div style={{ position: 'relative', display: 'flex', flexDirection: 'column', alignItems: 'center', zIndex: 10 }}>
        <span style={{ fontSize: 32, fontWeight: 700, color: '#ffffff' }}>🏢</span>
        <span style={{ fontSize: 11, color: 'rgba(255,255,255,0.4)', letterSpacing: 2, textTransform: 'uppercase', marginTop: 4 }}>ceo · vision studios</span>
      </div>
    </div>
  </div>
</div>
```

```aura width=800 height=340
<div style={{ position: 'relative', display: 'flex', flexDirection: 'column', width: '100%', height: '100%', background: '#08080d', borderRadius: 20, overflow: 'hidden', fontFamily: 'Inter, sans-serif', padding: '30px 36px' }}>
  <style>{`
    @keyframes prfa { 0%, 100% { transform: translate(0,0); opacity: 0.55; } 50% { transform: translate(20px,-14px); opacity: 0.85; } }
    @keyframes prfb { 0%, 100% { transform: translate(0,0); opacity: 0.45; } 50% { transform: translate(-16px,12px); opacity: 0.75; } }
    #pro1 { animation: prfa 10s ease-in-out infinite; }
    #pro2 { animation: prfb 12s ease-in-out infinite 1s; }
    #pro3 { animation: prfa 9s ease-in-out infinite 2.5s; }
    #pro4 { animation: prfb 11s ease-in-out infinite 0.5s; }
    @keyframes pr-pulse { 0%, 100% { opacity: 1; } 50% { opacity: 0.2; } }
    #pr-dot { animation: pr-pulse 1.6s ease-in-out infinite; }
  `}</style>
  <svg width="800" height="340" style={{ position: 'absolute', top: 0, left: 0 }}>
    <defs>
      <radialGradient id="prg1" cx="50%" cy="50%" r="50%"><stop offset="0%" stopColor="rgba(108,195,130,0.45)" /><stop offset="100%" stopColor="rgba(108,195,130,0)" /></radialGradient>
      <radialGradient id="prg2" cx="50%" cy="50%" r="50%"><stop offset="0%" stopColor="rgba(230,100,115,0.4)" /><stop offset="100%" stopColor="rgba(230,100,115,0)" /></radialGradient>
      <radialGradient id="prg3" cx="50%" cy="50%" r="50%"><stop offset="0%" stopColor="rgba(80,160,220,0.35)" /><stop offset="100%" stopColor="rgba(80,160,220,0)" /></radialGradient>
      <radialGradient id="prg4" cx="50%" cy="50%" r="50%"><stop offset="0%" stopColor="rgba(195,155,255,0.3)" /><stop offset="100%" stopColor="rgba(195,155,255,0)" /></radialGradient>
    </defs>
    <ellipse id="pro1" cx="90" cy="300" rx="200" ry="150" fill="url(#prg1)" />
    <ellipse id="pro2" cx="720" cy="60" rx="190" ry="150" fill="url(#prg2)" />
    <ellipse id="pro3" cx="640" cy="320" rx="180" ry="140" fill="url(#prg3)" />
    <ellipse id="pro4" cx="220" cy="40" rx="160" ry="120" fill="url(#prg4)" />
    <circle id="pr-dot" cx="578" cy="42" r="4" fill="#ffc36e" />
  </svg>
  <div style={{ display: 'flex', alignItems: 'center', justifyContent: 'space-between' }}>
    <span style={{ fontSize: 11, color: 'rgba(255,255,255,0.35)', letterSpacing: 4, textTransform: 'uppercase' }}>projeto mais recente</span>
    <div style={{ position: 'relative', display: 'flex', alignItems: 'center', padding: '5px 14px 5px 28px', borderRadius: 100, background: 'rgba(255,195,110,0.08)', border: '1px solid rgba(255,195,110,0.3)' }}>
      <span style={{ fontSize: 11, color: '#ffc36e', letterSpacing: 1.5, textTransform: 'uppercase' }}>em desenvolvimento</span>
    </div>
  </div>
  <span style={{ fontSize: 44, fontWeight: 700, color: '#ffffff', letterSpacing: -1.5, marginTop: 10, height: 58, display: 'flex', alignItems: 'center' }}>Prumoo</span>
  <span style={{ fontSize: 15, color: 'rgba(255,255,255,0.6)', marginTop: 6 }}>Gestão financeira pessoal com um time de agentes de IA trabalhando junto com você.</span>
  <div style={{ display: 'flex', flexWrap: 'wrap', gap: 14, marginTop: 20 }}>
      <div style={{ display: 'flex', flexDirection: 'column', padding: '14px 18px', background: 'rgba(255,255,255,0.035)', border: '1px solid rgba(255,255,255,0.08)', borderRadius: 14, width: 356 }}>
        <span style={{ fontSize: 14, fontWeight: 600, color: '#ffffff' }}>💸  Finanças completas</span>
        <span style={{ fontSize: 12, color: 'rgba(255,255,255,0.5)', marginTop: 4 }}>contas, cartões, faturas e recorrências</span>
      </div>
      <div style={{ display: 'flex', flexDirection: 'column', padding: '14px 18px', background: 'rgba(255,255,255,0.035)', border: '1px solid rgba(255,255,255,0.08)', borderRadius: 14, width: 356 }}>
        <span style={{ fontSize: 14, fontWeight: 600, color: '#ffffff' }}>🎯  Planejamento</span>
        <span style={{ fontSize: 12, color: 'rgba(255,255,255,0.5)', marginTop: 4 }}>orçamento, metas, patrimônio e relatórios</span>
      </div>
      <div style={{ display: 'flex', flexDirection: 'column', padding: '14px 18px', background: 'rgba(255,255,255,0.035)', border: '1px solid rgba(255,255,255,0.08)', borderRadius: 14, width: 356 }}>
        <span style={{ fontSize: 14, fontWeight: 600, color: '#ffffff' }}>🏦  Open Finance</span>
        <span style={{ fontSize: 12, color: 'rgba(255,255,255,0.5)', marginTop: 4 }}>conexão com bancos via Pluggy</span>
      </div>
      <div style={{ display: 'flex', flexDirection: 'column', padding: '14px 18px', background: 'rgba(255,255,255,0.035)', border: '1px solid rgba(255,255,255,0.08)', borderRadius: 14, width: 356 }}>
        <span style={{ fontSize: 14, fontWeight: 600, color: '#ffffff' }}>🤖  Squad de IA</span>
        <span style={{ fontSize: 12, color: 'rgba(255,255,255,0.5)', marginTop: 4 }}>8 agentes especialistas orquestrados via A2A</span>
      </div>
  </div>
  <span style={{ fontSize: 11, color: 'rgba(255,255,255,0.35)', marginTop: 16, letterSpacing: 0.5 }}>Next.js 16 · React 19 · Tailwind · shadcn/ui · Python · FastAPI · PostgreSQL · Docker</span>
</div>
```

```aura width=800 height=380
<div style={{ position: 'relative', display: 'flex', flexDirection: 'column', width: '100%', height: '100%', background: '#08080d', borderRadius: 20, overflow: 'hidden', fontFamily: 'Inter, sans-serif', padding: '30px 36px' }}>
  <style>{`
    @keyframes pjfa { 0%, 100% { transform: translate(0,0); opacity: 0.55; } 50% { transform: translate(20px,-14px); opacity: 0.85; } }
    @keyframes pjfb { 0%, 100% { transform: translate(0,0); opacity: 0.45; } 50% { transform: translate(-16px,12px); opacity: 0.75; } }
    #pjo1 { animation: pjfa 10s ease-in-out infinite; }
    #pjo2 { animation: pjfb 12s ease-in-out infinite 1s; }
    #pjo3 { animation: pjfa 9s ease-in-out infinite 2.5s; }
    #pjo4 { animation: pjfb 11s ease-in-out infinite 0.5s; }
  `}</style>
  <svg width="800" height="380" style={{ position: 'absolute', top: 0, left: 0 }}>
    <defs>
      <radialGradient id="pjg1" cx="50%" cy="50%" r="50%"><stop offset="0%" stopColor="rgba(108,195,130,0.45)" /><stop offset="100%" stopColor="rgba(108,195,130,0)" /></radialGradient>
      <radialGradient id="pjg2" cx="50%" cy="50%" r="50%"><stop offset="0%" stopColor="rgba(230,100,115,0.4)" /><stop offset="100%" stopColor="rgba(230,100,115,0)" /></radialGradient>
      <radialGradient id="pjg3" cx="50%" cy="50%" r="50%"><stop offset="0%" stopColor="rgba(80,160,220,0.35)" /><stop offset="100%" stopColor="rgba(80,160,220,0)" /></radialGradient>
      <radialGradient id="pjg4" cx="50%" cy="50%" r="50%"><stop offset="0%" stopColor="rgba(195,155,255,0.3)" /><stop offset="100%" stopColor="rgba(195,155,255,0)" /></radialGradient>
    </defs>
    <ellipse id="pjo1" cx="720" cy="340" rx="200" ry="150" fill="url(#pjg1)" />
    <ellipse id="pjo2" cx="80" cy="60" rx="190" ry="150" fill="url(#pjg2)" />
    <ellipse id="pjo3" cx="120" cy="360" rx="180" ry="140" fill="url(#pjg3)" />
    <ellipse id="pjo4" cx="600" cy="30" rx="160" ry="120" fill="url(#pjg4)" />
  </svg>
  <span style={{ fontSize: 11, color: 'rgba(255,255,255,0.35)', letterSpacing: 4, textTransform: 'uppercase' }}>projetos recentes</span>
  <span style={{ fontSize: 22, fontWeight: 600, color: '#ffffff', marginTop: 8 }}>O que eu venho construindo</span>
  <div style={{ display: 'flex', flexWrap: 'wrap', gap: 14, marginTop: 20 }}>
    <div style={{ display: 'flex', flexDirection: 'column', padding: '14px 18px', background: 'rgba(255,255,255,0.035)', border: '1px solid rgba(255,255,255,0.08)', borderRadius: 14, width: 356, height: 78 }}>
      <div style={{ display: 'flex', justifyContent: 'space-between', alignItems: 'center' }}>
        <span style={{ fontSize: 15, fontWeight: 600, color: '#ffffff' }}>Sistema Leal</span>
        <span style={{ fontSize: 10, color: 'rgba(255,255,255,0.4)', letterSpacing: 1 }}>🔒 PRIVADO</span>
      </div>
      <span style={{ fontSize: 12, color: 'rgba(255,255,255,0.55)', marginTop: 4 }}>Gestão de lideranças de campanha</span>
      <span style={{ fontSize: 11, color: 'rgba(108,195,130,0.8)', marginTop: 6 }}>React · AWS Lambda · Supabase</span>
    </div>
    <div style={{ display: 'flex', flexDirection: 'column', padding: '14px 18px', background: 'rgba(255,255,255,0.035)', border: '1px solid rgba(255,255,255,0.08)', borderRadius: 14, width: 356, height: 78 }}>
      <div style={{ display: 'flex', justifyContent: 'space-between', alignItems: 'center' }}>
        <span style={{ fontSize: 15, fontWeight: 600, color: '#ffffff' }}>Plenum</span>
        <span style={{ fontSize: 10, color: 'rgba(255,255,255,0.4)', letterSpacing: 1 }}>🔒 PRIVADO</span>
      </div>
      <span style={{ fontSize: 12, color: 'rgba(255,255,255,0.55)', marginTop: 4 }}>Escalas de acólitos e coroinhas</span>
      <span style={{ fontSize: 11, color: 'rgba(108,195,130,0.8)', marginTop: 6 }}>React · Lambda · Postgres</span>
    </div>
    <div style={{ display: 'flex', flexDirection: 'column', padding: '14px 18px', background: 'rgba(255,255,255,0.035)', border: '1px solid rgba(255,255,255,0.08)', borderRadius: 14, width: 356, height: 78 }}>
      <div style={{ display: 'flex', justifyContent: 'space-between', alignItems: 'center' }}>
        <span style={{ fontSize: 15, fontWeight: 600, color: '#ffffff' }}>Vision</span>
        <span style={{ fontSize: 10, color: 'rgba(255,255,255,0.4)', letterSpacing: 1 }}>🔒 PRIVADO</span>
      </div>
      <span style={{ fontSize: 12, color: 'rgba(255,255,255,0.55)', marginTop: 4 }}>Portfólio da Vision Studios</span>
      <span style={{ fontSize: 11, color: 'rgba(108,195,130,0.8)', marginTop: 6 }}>React · Vite · Tailwind</span>
    </div>
    <div style={{ display: 'flex', flexDirection: 'column', padding: '14px 18px', background: 'rgba(255,255,255,0.035)', border: '1px solid rgba(255,255,255,0.08)', borderRadius: 14, width: 356, height: 78 }}>
      <div style={{ display: 'flex', justifyContent: 'space-between', alignItems: 'center' }}>
        <span style={{ fontSize: 15, fontWeight: 600, color: '#ffffff' }}>Adv</span>
        <span style={{ fontSize: 10, color: 'rgba(255,255,255,0.4)', letterSpacing: 1 }}>🔒 PRIVADO</span>
      </div>
      <span style={{ fontSize: 12, color: 'rgba(255,255,255,0.55)', marginTop: 4 }}>Sistema para escritório de advocacia</span>
      <span style={{ fontSize: 11, color: 'rgba(108,195,130,0.8)', marginTop: 6 }}>React · TypeScript · Vite</span>
    </div>
    <div style={{ display: 'flex', flexDirection: 'column', padding: '14px 18px', background: 'rgba(255,255,255,0.035)', border: '1px solid rgba(255,255,255,0.08)', borderRadius: 14, width: 356, height: 78 }}>
      <div style={{ display: 'flex', justifyContent: 'space-between', alignItems: 'center' }}>
        <span style={{ fontSize: 15, fontWeight: 600, color: '#ffffff' }}>Lazaro Garcia Oficina</span>
        <span style={{ fontSize: 10, color: 'rgba(255,255,255,0.4)', letterSpacing: 1 }}>🔒 PRIVADO</span>
      </div>
      <span style={{ fontSize: 12, color: 'rgba(255,255,255,0.55)', marginTop: 4 }}>Gestão para oficina mecânica</span>
      <span style={{ fontSize: 11, color: 'rgba(108,195,130,0.8)', marginTop: 6 }}>TypeScript</span>
    </div>
    <div style={{ display: 'flex', flexDirection: 'column', padding: '14px 18px', background: 'rgba(255,255,255,0.035)', border: '1px solid rgba(255,255,255,0.08)', borderRadius: 14, width: 356, height: 78 }}>
      <div style={{ display: 'flex', justifyContent: 'space-between', alignItems: 'center' }}>
        <span style={{ fontSize: 15, fontWeight: 600, color: '#ffffff' }}>PedroPlay Downloader</span>
        <span style={{ fontSize: 10, color: 'rgba(255,255,255,0.4)', letterSpacing: 1 }}>🔒 PRIVADO</span>
      </div>
      <span style={{ fontSize: 12, color: 'rgba(255,255,255,0.55)', marginTop: 4 }}>Baixa vídeos, corta trechos e gera MP3</span>
      <span style={{ fontSize: 11, color: 'rgba(108,195,130,0.8)', marginTop: 6 }}>Next.js · yt-dlp</span>
    </div>
  </div>
</div>
```

```aura width=800 height=304
<div style={{ position: 'relative', display: 'flex', flexDirection: 'column', width: '100%', height: '100%', background: '#08080d', borderRadius: 20, overflow: 'hidden', fontFamily: 'Inter, sans-serif', padding: '30px 36px' }}>
  <style>{`
    @keyframes rtfa { 0%, 100% { transform: translate(0,0); opacity: 0.55; } 50% { transform: translate(20px,-14px); opacity: 0.85; } }
    @keyframes rtfb { 0%, 100% { transform: translate(0,0); opacity: 0.45; } 50% { transform: translate(-16px,12px); opacity: 0.75; } }
    #rto1 { animation: rtfa 10s ease-in-out infinite; }
    #rto2 { animation: rtfb 12s ease-in-out infinite 1s; }
    #rto3 { animation: rtfa 9s ease-in-out infinite 2.5s; }
    #rto4 { animation: rtfb 11s ease-in-out infinite 0.5s; }
    @keyframes rt-scan { 0% { transform: translateX(0); opacity: 0; } 10% { opacity: 0.9; } 90% { opacity: 0.9; } 100% { transform: translateX(686px); opacity: 0; } }
    #rt-scan { animation: rt-scan 6s linear infinite; }
  `}</style>
  <svg width="800" height="304" style={{ position: 'absolute', top: 0, left: 0 }}>
    <defs>
      <radialGradient id="rtg1" cx="50%" cy="50%" r="50%"><stop offset="0%" stopColor="rgba(108,195,130,0.45)" /><stop offset="100%" stopColor="rgba(108,195,130,0)" /></radialGradient>
      <radialGradient id="rtg2" cx="50%" cy="50%" r="50%"><stop offset="0%" stopColor="rgba(230,100,115,0.4)" /><stop offset="100%" stopColor="rgba(230,100,115,0)" /></radialGradient>
      <radialGradient id="rtg3" cx="50%" cy="50%" r="50%"><stop offset="0%" stopColor="rgba(80,160,220,0.35)" /><stop offset="100%" stopColor="rgba(80,160,220,0)" /></radialGradient>
      <radialGradient id="rtg4" cx="50%" cy="50%" r="50%"><stop offset="0%" stopColor="rgba(195,155,255,0.3)" /><stop offset="100%" stopColor="rgba(195,155,255,0)" /></radialGradient>
    </defs>
    <ellipse id="rto1" cx="100" cy="40" rx="200" ry="150" fill="url(#rtg1)" />
    <ellipse id="rto2" cx="700" cy="300" rx="190" ry="150" fill="url(#rtg2)" />
    <ellipse id="rto3" cx="740" cy="50" rx="180" ry="140" fill="url(#rtg3)" />
    <ellipse id="rto4" cx="300" cy="320" rx="160" ry="120" fill="url(#rtg4)" />
  </svg>
  <span style={{ fontSize: 11, color: 'rgba(255,255,255,0.35)', letterSpacing: 4, textTransform: 'uppercase' }}>ritmo</span>
  <div style={{ display: 'flex', gap: 14, marginTop: 14 }}>
    <div style={{ display: 'flex', flexDirection: 'column', padding: '14px 18px', background: 'rgba(255,255,255,0.035)', border: '1px solid rgba(255,255,255,0.08)', borderRadius: 14, width: 172, alignItems: 'center' }}>
      <span style={{ fontSize: 26, fontWeight: 700, color: '#ffffff' }}>{(github && github.stats && github.user ? github.stats.totalRepos : 30)}</span>
      <span style={{ fontSize: 11, color: 'rgba(255,255,255,0.45)', marginTop: 2 }}>repositórios públicos</span>
    </div>
    <div style={{ display: 'flex', flexDirection: 'column', padding: '14px 18px', background: 'rgba(255,255,255,0.035)', border: '1px solid rgba(255,255,255,0.08)', borderRadius: 14, width: 172, alignItems: 'center' }}>
      <span style={{ fontSize: 26, fontWeight: 700, color: '#ffffff' }}>{(github && github.stats && github.user ? github.stats.totalStars : 5)}</span>
      <span style={{ fontSize: 11, color: 'rgba(255,255,255,0.45)', marginTop: 2 }}>estrelas</span>
    </div>
    <div style={{ display: 'flex', flexDirection: 'column', padding: '14px 18px', background: 'rgba(255,255,255,0.035)', border: '1px solid rgba(255,255,255,0.08)', borderRadius: 14, width: 172, alignItems: 'center' }}>
      <span style={{ fontSize: 26, fontWeight: 700, color: '#ffffff' }}>{(github && github.stats && github.user ? github.user.followers : 5)}</span>
      <span style={{ fontSize: 11, color: 'rgba(255,255,255,0.45)', marginTop: 2 }}>seguidores</span>
    </div>
    <div style={{ display: 'flex', flexDirection: 'column', padding: '14px 18px', background: 'rgba(255,255,255,0.035)', border: '1px solid rgba(255,255,255,0.08)', borderRadius: 14, width: 172, alignItems: 'center' }}>
      <span style={{ fontSize: 26, fontWeight: 700, color: '#ffffff' }}>{36}</span>
      <span style={{ fontSize: 11, color: 'rgba(255,255,255,0.45)', marginTop: 2 }}>contribuições no ano</span>
    </div>
  </div>
  <div style={{ display: 'flex', justifyContent: 'space-between', alignItems: 'center', marginTop: 22 }}>
    <span style={{ fontSize: 13, color: 'rgba(255,255,255,0.6)' }}>Atividade de contribuições</span>
    <div style={{ display: 'flex', alignItems: 'center' }}>
      <span style={{ fontSize: 10, color: 'rgba(255,255,255,0.4)', marginRight: 87 }}>menos</span>
      <span style={{ fontSize: 10, color: 'rgba(255,255,255,0.4)' }}>mais</span>
    </div>
  </div>
  <svg width="800" height="304" style={{ position: 'absolute', top: 0, left: 0 }}>
    <g transform="translate(659, 158)"><rect x="0" y="0" width="10" height="10" rx="2.5" fill="rgba(255,255,255,0.05)" /><rect x="15" y="0" width="10" height="10" rx="2.5" fill="rgba(108,195,130,0.35)" /><rect x="30" y="0" width="10" height="10" rx="2.5" fill="rgba(108,195,130,0.55)" /><rect x="45" y="0" width="10" height="10" rx="2.5" fill="rgba(108,195,130,0.8)" /><rect x="60" y="0" width="10" height="10" rx="2.5" fill="rgba(140,230,165,1)" /></g>
    <g transform="translate(57, 186)">
      <rect x="0" y="0" width="10" height="10" rx="2.5" fill="rgba(255,255,255,0.05)" /><rect x="0" y="13" width="10" height="10" rx="2.5" fill="rgba(255,255,255,0.05)" /><rect x="0" y="26" width="10" height="10" rx="2.5" fill="rgba(255,255,255,0.05)" /><rect x="0" y="39" width="10" height="10" rx="2.5" fill="rgba(255,255,255,0.05)" /><rect x="0" y="52" width="10" height="10" rx="2.5" fill="rgba(255,255,255,0.05)" /><rect x="0" y="65" width="10" height="10" rx="2.5" fill="rgba(255,255,255,0.05)" /><rect x="0" y="78" width="10" height="10" rx="2.5" fill="rgba(255,255,255,0.05)" /><rect x="13" y="0" width="10" height="10" rx="2.5" fill="rgba(255,255,255,0.05)" /><rect x="13" y="13" width="10" height="10" rx="2.5" fill="rgba(255,255,255,0.05)" /><rect x="13" y="26" width="10" height="10" rx="2.5" fill="rgba(255,255,255,0.05)" /><rect x="13" y="39" width="10" height="10" rx="2.5" fill="rgba(255,255,255,0.05)" /><rect x="13" y="52" width="10" height="10" rx="2.5" fill="rgba(255,255,255,0.05)" /><rect x="13" y="65" width="10" height="10" rx="2.5" fill="rgba(255,255,255,0.05)" /><rect x="13" y="78" width="10" height="10" rx="2.5" fill="rgba(255,255,255,0.05)" /><rect x="26" y="0" width="10" height="10" rx="2.5" fill="rgba(255,255,255,0.05)" /><rect x="26" y="13" width="10" height="10" rx="2.5" fill="rgba(255,255,255,0.05)" /><rect x="26" y="26" width="10" height="10" rx="2.5" fill="rgba(255,255,255,0.05)" /><rect x="26" y="39" width="10" height="10" rx="2.5" fill="rgba(255,255,255,0.05)" /><rect x="26" y="52" width="10" height="10" rx="2.5" fill="rgba(255,255,255,0.05)" /><rect x="26" y="65" width="10" height="10" rx="2.5" fill="rgba(255,255,255,0.05)" /><rect x="26" y="78" width="10" height="10" rx="2.5" fill="rgba(255,255,255,0.05)" /><rect x="39" y="0" width="10" height="10" rx="2.5" fill="rgba(255,255,255,0.05)" /><rect x="39" y="13" width="10" height="10" rx="2.5" fill="rgba(255,255,255,0.05)" /><rect x="39" y="26" width="10" height="10" rx="2.5" fill="rgba(255,255,255,0.05)" /><rect x="39" y="39" width="10" height="10" rx="2.5" fill="rgba(255,255,255,0.05)" /><rect x="39" y="52" width="10" height="10" rx="2.5" fill="rgba(255,255,255,0.05)" /><rect x="39" y="65" width="10" height="10" rx="2.5" fill="rgba(255,255,255,0.05)" /><rect x="39" y="78" width="10" height="10" rx="2.5" fill="rgba(255,255,255,0.05)" /><rect x="52" y="0" width="10" height="10" rx="2.5" fill="rgba(255,255,255,0.05)" /><rect x="52" y="13" width="10" height="10" rx="2.5" fill="rgba(255,255,255,0.05)" /><rect x="52" y="26" width="10" height="10" rx="2.5" fill="rgba(255,255,255,0.05)" /><rect x="52" y="39" width="10" height="10" rx="2.5" fill="rgba(255,255,255,0.05)" /><rect x="52" y="52" width="10" height="10" rx="2.5" fill="rgba(255,255,255,0.05)" /><rect x="52" y="65" width="10" height="10" rx="2.5" fill="rgba(255,255,255,0.05)" /><rect x="52" y="78" width="10" height="10" rx="2.5" fill="rgba(255,255,255,0.05)" /><rect x="65" y="0" width="10" height="10" rx="2.5" fill="rgba(255,255,255,0.05)" /><rect x="65" y="13" width="10" height="10" rx="2.5" fill="rgba(255,255,255,0.05)" /><rect x="65" y="26" width="10" height="10" rx="2.5" fill="rgba(255,255,255,0.05)" /><rect x="65" y="39" width="10" height="10" rx="2.5" fill="rgba(255,255,255,0.05)" /><rect x="65" y="52" width="10" height="10" rx="2.5" fill="rgba(255,255,255,0.05)" /><rect x="65" y="65" width="10" height="10" rx="2.5" fill="rgba(255,255,255,0.05)" /><rect x="65" y="78" width="10" height="10" rx="2.5" fill="rgba(255,255,255,0.05)" /><rect x="78" y="0" width="10" height="10" rx="2.5" fill="rgba(255,255,255,0.05)" /><rect x="78" y="13" width="10" height="10" rx="2.5" fill="rgba(255,255,255,0.05)" /><rect x="78" y="26" width="10" height="10" rx="2.5" fill="rgba(255,255,255,0.05)" /><rect x="78" y="39" width="10" height="10" rx="2.5" fill="rgba(255,255,255,0.05)" /><rect x="78" y="52" width="10" height="10" rx="2.5" fill="rgba(255,255,255,0.05)" /><rect x="78" y="65" width="10" height="10" rx="2.5" fill="rgba(255,255,255,0.05)" /><rect x="78" y="78" width="10" height="10" rx="2.5" fill="rgba(255,255,255,0.05)" /><rect x="91" y="0" width="10" height="10" rx="2.5" fill="rgba(255,255,255,0.05)" /><rect x="91" y="13" width="10" height="10" rx="2.5" fill="rgba(255,255,255,0.05)" /><rect x="91" y="26" width="10" height="10" rx="2.5" fill="rgba(255,255,255,0.05)" /><rect x="91" y="39" width="10" height="10" rx="2.5" fill="rgba(255,255,255,0.05)" /><rect x="91" y="52" width="10" height="10" rx="2.5" fill="rgba(255,255,255,0.05)" /><rect x="91" y="65" width="10" height="10" rx="2.5" fill="rgba(255,255,255,0.05)" /><rect x="91" y="78" width="10" height="10" rx="2.5" fill="rgba(255,255,255,0.05)" /><rect x="104" y="0" width="10" height="10" rx="2.5" fill="rgba(255,255,255,0.05)" /><rect x="104" y="13" width="10" height="10" rx="2.5" fill="rgba(255,255,255,0.05)" /><rect x="104" y="26" width="10" height="10" rx="2.5" fill="rgba(255,255,255,0.05)" /><rect x="104" y="39" width="10" height="10" rx="2.5" fill="rgba(255,255,255,0.05)" /><rect x="104" y="52" width="10" height="10" rx="2.5" fill="rgba(255,255,255,0.05)" /><rect x="104" y="65" width="10" height="10" rx="2.5" fill="rgba(255,255,255,0.05)" /><rect x="104" y="78" width="10" height="10" rx="2.5" fill="rgba(255,255,255,0.05)" /><rect x="117" y="0" width="10" height="10" rx="2.5" fill="rgba(255,255,255,0.05)" /><rect x="117" y="13" width="10" height="10" rx="2.5" fill="rgba(255,255,255,0.05)" /><rect x="117" y="26" width="10" height="10" rx="2.5" fill="rgba(255,255,255,0.05)" /><rect x="117" y="39" width="10" height="10" rx="2.5" fill="rgba(255,255,255,0.05)" /><rect x="117" y="52" width="10" height="10" rx="2.5" fill="rgba(255,255,255,0.05)" /><rect x="117" y="65" width="10" height="10" rx="2.5" fill="rgba(255,255,255,0.05)" /><rect x="117" y="78" width="10" height="10" rx="2.5" fill="rgba(255,255,255,0.05)" /><rect x="130" y="0" width="10" height="10" rx="2.5" fill="rgba(255,255,255,0.05)" /><rect x="130" y="13" width="10" height="10" rx="2.5" fill="rgba(255,255,255,0.05)" /><rect x="130" y="26" width="10" height="10" rx="2.5" fill="rgba(255,255,255,0.05)" /><rect x="130" y="39" width="10" height="10" rx="2.5" fill="rgba(255,255,255,0.05)" /><rect x="130" y="52" width="10" height="10" rx="2.5" fill="rgba(255,255,255,0.05)" /><rect x="130" y="65" width="10" height="10" rx="2.5" fill="rgba(255,255,255,0.05)" /><rect x="130" y="78" width="10" height="10" rx="2.5" fill="rgba(255,255,255,0.05)" /><rect x="143" y="0" width="10" height="10" rx="2.5" fill="rgba(255,255,255,0.05)" /><rect x="143" y="13" width="10" height="10" rx="2.5" fill="rgba(255,255,255,0.05)" /><rect x="143" y="26" width="10" height="10" rx="2.5" fill="rgba(255,255,255,0.05)" /><rect x="143" y="39" width="10" height="10" rx="2.5" fill="rgba(255,255,255,0.05)" /><rect x="143" y="52" width="10" height="10" rx="2.5" fill="rgba(255,255,255,0.05)" /><rect x="143" y="65" width="10" height="10" rx="2.5" fill="rgba(255,255,255,0.05)" /><rect x="143" y="78" width="10" height="10" rx="2.5" fill="rgba(255,255,255,0.05)" /><rect x="156" y="0" width="10" height="10" rx="2.5" fill="rgba(255,255,255,0.05)" /><rect x="156" y="13" width="10" height="10" rx="2.5" fill="rgba(255,255,255,0.05)" /><rect x="156" y="26" width="10" height="10" rx="2.5" fill="rgba(255,255,255,0.05)" /><rect x="156" y="39" width="10" height="10" rx="2.5" fill="rgba(255,255,255,0.05)" /><rect x="156" y="52" width="10" height="10" rx="2.5" fill="rgba(255,255,255,0.05)" /><rect x="156" y="65" width="10" height="10" rx="2.5" fill="rgba(255,255,255,0.05)" /><rect x="156" y="78" width="10" height="10" rx="2.5" fill="rgba(255,255,255,0.05)" /><rect x="169" y="0" width="10" height="10" rx="2.5" fill="rgba(255,255,255,0.05)" /><rect x="169" y="13" width="10" height="10" rx="2.5" fill="rgba(255,255,255,0.05)" /><rect x="169" y="26" width="10" height="10" rx="2.5" fill="rgba(255,255,255,0.05)" /><rect x="169" y="39" width="10" height="10" rx="2.5" fill="rgba(255,255,255,0.05)" /><rect x="169" y="52" width="10" height="10" rx="2.5" fill="rgba(255,255,255,0.05)" /><rect x="169" y="65" width="10" height="10" rx="2.5" fill="rgba(255,255,255,0.05)" /><rect x="169" y="78" width="10" height="10" rx="2.5" fill="rgba(255,255,255,0.05)" /><rect x="182" y="0" width="10" height="10" rx="2.5" fill="rgba(255,255,255,0.05)" /><rect x="182" y="13" width="10" height="10" rx="2.5" fill="rgba(255,255,255,0.05)" /><rect x="182" y="26" width="10" height="10" rx="2.5" fill="rgba(255,255,255,0.05)" /><rect x="182" y="39" width="10" height="10" rx="2.5" fill="rgba(255,255,255,0.05)" /><rect x="182" y="52" width="10" height="10" rx="2.5" fill="rgba(255,255,255,0.05)" /><rect x="182" y="65" width="10" height="10" rx="2.5" fill="rgba(255,255,255,0.05)" /><rect x="182" y="78" width="10" height="10" rx="2.5" fill="rgba(255,255,255,0.05)" /><rect x="195" y="0" width="10" height="10" rx="2.5" fill="rgba(255,255,255,0.05)" /><rect x="195" y="13" width="10" height="10" rx="2.5" fill="rgba(255,255,255,0.05)" /><rect x="195" y="26" width="10" height="10" rx="2.5" fill="rgba(255,255,255,0.05)" /><rect x="195" y="39" width="10" height="10" rx="2.5" fill="rgba(255,255,255,0.05)" /><rect x="195" y="52" width="10" height="10" rx="2.5" fill="rgba(255,255,255,0.05)" /><rect x="195" y="65" width="10" height="10" rx="2.5" fill="rgba(255,255,255,0.05)" /><rect x="195" y="78" width="10" height="10" rx="2.5" fill="rgba(255,255,255,0.05)" /><rect x="208" y="0" width="10" height="10" rx="2.5" fill="rgba(255,255,255,0.05)" /><rect x="208" y="13" width="10" height="10" rx="2.5" fill="rgba(255,255,255,0.05)" /><rect x="208" y="26" width="10" height="10" rx="2.5" fill="rgba(255,255,255,0.05)" /><rect x="208" y="39" width="10" height="10" rx="2.5" fill="rgba(255,255,255,0.05)" /><rect x="208" y="52" width="10" height="10" rx="2.5" fill="rgba(255,255,255,0.05)" /><rect x="208" y="65" width="10" height="10" rx="2.5" fill="rgba(255,255,255,0.05)" /><rect x="208" y="78" width="10" height="10" rx="2.5" fill="rgba(255,255,255,0.05)" /><rect x="221" y="0" width="10" height="10" rx="2.5" fill="rgba(255,255,255,0.05)" /><rect x="221" y="13" width="10" height="10" rx="2.5" fill="rgba(255,255,255,0.05)" /><rect x="221" y="26" width="10" height="10" rx="2.5" fill="rgba(255,255,255,0.05)" /><rect x="221" y="39" width="10" height="10" rx="2.5" fill="rgba(255,255,255,0.05)" /><rect x="221" y="52" width="10" height="10" rx="2.5" fill="rgba(255,255,255,0.05)" /><rect x="221" y="65" width="10" height="10" rx="2.5" fill="rgba(255,255,255,0.05)" /><rect x="221" y="78" width="10" height="10" rx="2.5" fill="rgba(255,255,255,0.05)" /><rect x="234" y="0" width="10" height="10" rx="2.5" fill="rgba(255,255,255,0.05)" /><rect x="234" y="13" width="10" height="10" rx="2.5" fill="rgba(255,255,255,0.05)" /><rect x="234" y="26" width="10" height="10" rx="2.5" fill="rgba(255,255,255,0.05)" /><rect x="234" y="39" width="10" height="10" rx="2.5" fill="rgba(255,255,255,0.05)" /><rect x="234" y="52" width="10" height="10" rx="2.5" fill="rgba(255,255,255,0.05)" /><rect x="234" y="65" width="10" height="10" rx="2.5" fill="rgba(255,255,255,0.05)" /><rect x="234" y="78" width="10" height="10" rx="2.5" fill="rgba(255,255,255,0.05)" /><rect x="247" y="0" width="10" height="10" rx="2.5" fill="rgba(255,255,255,0.05)" /><rect x="247" y="13" width="10" height="10" rx="2.5" fill="rgba(255,255,255,0.05)" /><rect x="247" y="26" width="10" height="10" rx="2.5" fill="rgba(255,255,255,0.05)" /><rect x="247" y="39" width="10" height="10" rx="2.5" fill="rgba(255,255,255,0.05)" /><rect x="247" y="52" width="10" height="10" rx="2.5" fill="rgba(255,255,255,0.05)" /><rect x="247" y="65" width="10" height="10" rx="2.5" fill="rgba(255,255,255,0.05)" /><rect x="247" y="78" width="10" height="10" rx="2.5" fill="rgba(255,255,255,0.05)" /><rect x="260" y="0" width="10" height="10" rx="2.5" fill="rgba(255,255,255,0.05)" /><rect x="260" y="13" width="10" height="10" rx="2.5" fill="rgba(255,255,255,0.05)" /><rect x="260" y="26" width="10" height="10" rx="2.5" fill="rgba(255,255,255,0.05)" /><rect x="260" y="39" width="10" height="10" rx="2.5" fill="rgba(255,255,255,0.05)" /><rect x="260" y="52" width="10" height="10" rx="2.5" fill="rgba(255,255,255,0.05)" /><rect x="260" y="65" width="10" height="10" rx="2.5" fill="rgba(255,255,255,0.05)" /><rect x="260" y="78" width="10" height="10" rx="2.5" fill="rgba(255,255,255,0.05)" /><rect x="273" y="0" width="10" height="10" rx="2.5" fill="rgba(255,255,255,0.05)" /><rect x="273" y="13" width="10" height="10" rx="2.5" fill="rgba(255,255,255,0.05)" /><rect x="273" y="26" width="10" height="10" rx="2.5" fill="rgba(255,255,255,0.05)" /><rect x="273" y="39" width="10" height="10" rx="2.5" fill="rgba(255,255,255,0.05)" /><rect x="273" y="52" width="10" height="10" rx="2.5" fill="rgba(255,255,255,0.05)" /><rect x="273" y="65" width="10" height="10" rx="2.5" fill="rgba(255,255,255,0.05)" /><rect x="273" y="78" width="10" height="10" rx="2.5" fill="rgba(255,255,255,0.05)" /><rect x="286" y="0" width="10" height="10" rx="2.5" fill="rgba(255,255,255,0.05)" /><rect x="286" y="13" width="10" height="10" rx="2.5" fill="rgba(255,255,255,0.05)" /><rect x="286" y="26" width="10" height="10" rx="2.5" fill="rgba(255,255,255,0.05)" /><rect x="286" y="39" width="10" height="10" rx="2.5" fill="rgba(255,255,255,0.05)" /><rect x="286" y="52" width="10" height="10" rx="2.5" fill="rgba(255,255,255,0.05)" /><rect x="286" y="65" width="10" height="10" rx="2.5" fill="rgba(255,255,255,0.05)" /><rect x="286" y="78" width="10" height="10" rx="2.5" fill="rgba(255,255,255,0.05)" /><rect x="299" y="0" width="10" height="10" rx="2.5" fill="rgba(255,255,255,0.05)" /><rect x="299" y="13" width="10" height="10" rx="2.5" fill="rgba(255,255,255,0.05)" /><rect x="299" y="26" width="10" height="10" rx="2.5" fill="rgba(255,255,255,0.05)" /><rect x="299" y="39" width="10" height="10" rx="2.5" fill="rgba(255,255,255,0.05)" /><rect x="299" y="52" width="10" height="10" rx="2.5" fill="rgba(255,255,255,0.05)" /><rect x="299" y="65" width="10" height="10" rx="2.5" fill="rgba(255,255,255,0.05)" /><rect x="299" y="78" width="10" height="10" rx="2.5" fill="rgba(255,255,255,0.05)" /><rect x="312" y="0" width="10" height="10" rx="2.5" fill="rgba(255,255,255,0.05)" /><rect x="312" y="13" width="10" height="10" rx="2.5" fill="rgba(255,255,255,0.05)" /><rect x="312" y="26" width="10" height="10" rx="2.5" fill="rgba(255,255,255,0.05)" /><rect x="312" y="39" width="10" height="10" rx="2.5" fill="rgba(255,255,255,0.05)" /><rect x="312" y="52" width="10" height="10" rx="2.5" fill="rgba(255,255,255,0.05)" /><rect x="312" y="65" width="10" height="10" rx="2.5" fill="rgba(255,255,255,0.05)" /><rect x="312" y="78" width="10" height="10" rx="2.5" fill="rgba(255,255,255,0.05)" /><rect x="325" y="0" width="10" height="10" rx="2.5" fill="rgba(255,255,255,0.05)" /><rect x="325" y="13" width="10" height="10" rx="2.5" fill="rgba(255,255,255,0.05)" /><rect x="325" y="26" width="10" height="10" rx="2.5" fill="rgba(255,255,255,0.05)" /><rect x="325" y="39" width="10" height="10" rx="2.5" fill="rgba(255,255,255,0.05)" /><rect x="325" y="52" width="10" height="10" rx="2.5" fill="rgba(255,255,255,0.05)" /><rect x="325" y="65" width="10" height="10" rx="2.5" fill="rgba(255,255,255,0.05)" /><rect x="325" y="78" width="10" height="10" rx="2.5" fill="rgba(255,255,255,0.05)" /><rect x="338" y="0" width="10" height="10" rx="2.5" fill="rgba(255,255,255,0.05)" /><rect x="338" y="13" width="10" height="10" rx="2.5" fill="rgba(255,255,255,0.05)" /><rect x="338" y="26" width="10" height="10" rx="2.5" fill="rgba(255,255,255,0.05)" /><rect x="338" y="39" width="10" height="10" rx="2.5" fill="rgba(255,255,255,0.05)" /><rect x="338" y="52" width="10" height="10" rx="2.5" fill="rgba(255,255,255,0.05)" /><rect x="338" y="65" width="10" height="10" rx="2.5" fill="rgba(255,255,255,0.05)" /><rect x="338" y="78" width="10" height="10" rx="2.5" fill="rgba(255,255,255,0.05)" /><rect x="351" y="0" width="10" height="10" rx="2.5" fill="rgba(255,255,255,0.05)" /><rect x="351" y="13" width="10" height="10" rx="2.5" fill="rgba(255,255,255,0.05)" /><rect x="351" y="26" width="10" height="10" rx="2.5" fill="rgba(108,195,130,0.55)" /><rect x="351" y="39" width="10" height="10" rx="2.5" fill="rgba(140,230,165,1)" /><rect x="351" y="52" width="10" height="10" rx="2.5" fill="rgba(255,255,255,0.05)" /><rect x="351" y="65" width="10" height="10" rx="2.5" fill="rgba(255,255,255,0.05)" /><rect x="351" y="78" width="10" height="10" rx="2.5" fill="rgba(255,255,255,0.05)" /><rect x="364" y="0" width="10" height="10" rx="2.5" fill="rgba(255,255,255,0.05)" /><rect x="364" y="13" width="10" height="10" rx="2.5" fill="rgba(255,255,255,0.05)" /><rect x="364" y="26" width="10" height="10" rx="2.5" fill="rgba(255,255,255,0.05)" /><rect x="364" y="39" width="10" height="10" rx="2.5" fill="rgba(255,255,255,0.05)" /><rect x="364" y="52" width="10" height="10" rx="2.5" fill="rgba(255,255,255,0.05)" /><rect x="364" y="65" width="10" height="10" rx="2.5" fill="rgba(255,255,255,0.05)" /><rect x="364" y="78" width="10" height="10" rx="2.5" fill="rgba(255,255,255,0.05)" /><rect x="377" y="0" width="10" height="10" rx="2.5" fill="rgba(255,255,255,0.05)" /><rect x="377" y="13" width="10" height="10" rx="2.5" fill="rgba(255,255,255,0.05)" /><rect x="377" y="26" width="10" height="10" rx="2.5" fill="rgba(255,255,255,0.05)" /><rect x="377" y="39" width="10" height="10" rx="2.5" fill="rgba(255,255,255,0.05)" /><rect x="377" y="52" width="10" height="10" rx="2.5" fill="rgba(255,255,255,0.05)" /><rect x="377" y="65" width="10" height="10" rx="2.5" fill="rgba(255,255,255,0.05)" /><rect x="377" y="78" width="10" height="10" rx="2.5" fill="rgba(255,255,255,0.05)" /><rect x="390" y="0" width="10" height="10" rx="2.5" fill="rgba(255,255,255,0.05)" /><rect x="390" y="13" width="10" height="10" rx="2.5" fill="rgba(255,255,255,0.05)" /><rect x="390" y="26" width="10" height="10" rx="2.5" fill="rgba(255,255,255,0.05)" /><rect x="390" y="39" width="10" height="10" rx="2.5" fill="rgba(255,255,255,0.05)" /><rect x="390" y="52" width="10" height="10" rx="2.5" fill="rgba(255,255,255,0.05)" /><rect x="390" y="65" width="10" height="10" rx="2.5" fill="rgba(255,255,255,0.05)" /><rect x="390" y="78" width="10" height="10" rx="2.5" fill="rgba(255,255,255,0.05)" /><rect x="403" y="0" width="10" height="10" rx="2.5" fill="rgba(255,255,255,0.05)" /><rect x="403" y="13" width="10" height="10" rx="2.5" fill="rgba(255,255,255,0.05)" /><rect x="403" y="26" width="10" height="10" rx="2.5" fill="rgba(255,255,255,0.05)" /><rect x="403" y="39" width="10" height="10" rx="2.5" fill="rgba(255,255,255,0.05)" /><rect x="403" y="52" width="10" height="10" rx="2.5" fill="rgba(255,255,255,0.05)" /><rect x="403" y="65" width="10" height="10" rx="2.5" fill="rgba(255,255,255,0.05)" /><rect x="403" y="78" width="10" height="10" rx="2.5" fill="rgba(255,255,255,0.05)" /><rect x="416" y="0" width="10" height="10" rx="2.5" fill="rgba(255,255,255,0.05)" /><rect x="416" y="13" width="10" height="10" rx="2.5" fill="rgba(255,255,255,0.05)" /><rect x="416" y="26" width="10" height="10" rx="2.5" fill="rgba(255,255,255,0.05)" /><rect x="416" y="39" width="10" height="10" rx="2.5" fill="rgba(255,255,255,0.05)" /><rect x="416" y="52" width="10" height="10" rx="2.5" fill="rgba(255,255,255,0.05)" /><rect x="416" y="65" width="10" height="10" rx="2.5" fill="rgba(255,255,255,0.05)" /><rect x="416" y="78" width="10" height="10" rx="2.5" fill="rgba(255,255,255,0.05)" /><rect x="429" y="0" width="10" height="10" rx="2.5" fill="rgba(255,255,255,0.05)" /><rect x="429" y="13" width="10" height="10" rx="2.5" fill="rgba(255,255,255,0.05)" /><rect x="429" y="26" width="10" height="10" rx="2.5" fill="rgba(255,255,255,0.05)" /><rect x="429" y="39" width="10" height="10" rx="2.5" fill="rgba(255,255,255,0.05)" /><rect x="429" y="52" width="10" height="10" rx="2.5" fill="rgba(255,255,255,0.05)" /><rect x="429" y="65" width="10" height="10" rx="2.5" fill="rgba(255,255,255,0.05)" /><rect x="429" y="78" width="10" height="10" rx="2.5" fill="rgba(255,255,255,0.05)" /><rect x="442" y="0" width="10" height="10" rx="2.5" fill="rgba(255,255,255,0.05)" /><rect x="442" y="13" width="10" height="10" rx="2.5" fill="rgba(255,255,255,0.05)" /><rect x="442" y="26" width="10" height="10" rx="2.5" fill="rgba(255,255,255,0.05)" /><rect x="442" y="39" width="10" height="10" rx="2.5" fill="rgba(255,255,255,0.05)" /><rect x="442" y="52" width="10" height="10" rx="2.5" fill="rgba(255,255,255,0.05)" /><rect x="442" y="65" width="10" height="10" rx="2.5" fill="rgba(255,255,255,0.05)" /><rect x="442" y="78" width="10" height="10" rx="2.5" fill="rgba(255,255,255,0.05)" /><rect x="455" y="0" width="10" height="10" rx="2.5" fill="rgba(255,255,255,0.05)" /><rect x="455" y="13" width="10" height="10" rx="2.5" fill="rgba(255,255,255,0.05)" /><rect x="455" y="26" width="10" height="10" rx="2.5" fill="rgba(255,255,255,0.05)" /><rect x="455" y="39" width="10" height="10" rx="2.5" fill="rgba(255,255,255,0.05)" /><rect x="455" y="52" width="10" height="10" rx="2.5" fill="rgba(255,255,255,0.05)" /><rect x="455" y="65" width="10" height="10" rx="2.5" fill="rgba(255,255,255,0.05)" /><rect x="455" y="78" width="10" height="10" rx="2.5" fill="rgba(255,255,255,0.05)" /><rect x="468" y="0" width="10" height="10" rx="2.5" fill="rgba(255,255,255,0.05)" /><rect x="468" y="13" width="10" height="10" rx="2.5" fill="rgba(255,255,255,0.05)" /><rect x="468" y="26" width="10" height="10" rx="2.5" fill="rgba(255,255,255,0.05)" /><rect x="468" y="39" width="10" height="10" rx="2.5" fill="rgba(255,255,255,0.05)" /><rect x="468" y="52" width="10" height="10" rx="2.5" fill="rgba(255,255,255,0.05)" /><rect x="468" y="65" width="10" height="10" rx="2.5" fill="rgba(255,255,255,0.05)" /><rect x="468" y="78" width="10" height="10" rx="2.5" fill="rgba(255,255,255,0.05)" /><rect x="481" y="0" width="10" height="10" rx="2.5" fill="rgba(255,255,255,0.05)" /><rect x="481" y="13" width="10" height="10" rx="2.5" fill="rgba(108,195,130,0.8)" /><rect x="481" y="26" width="10" height="10" rx="2.5" fill="rgba(255,255,255,0.05)" /><rect x="481" y="39" width="10" height="10" rx="2.5" fill="rgba(255,255,255,0.05)" /><rect x="481" y="52" width="10" height="10" rx="2.5" fill="rgba(255,255,255,0.05)" /><rect x="481" y="65" width="10" height="10" rx="2.5" fill="rgba(140,230,165,1)" /><rect x="481" y="78" width="10" height="10" rx="2.5" fill="rgba(255,255,255,0.05)" /><rect x="494" y="0" width="10" height="10" rx="2.5" fill="rgba(108,195,130,0.55)" /><rect x="494" y="13" width="10" height="10" rx="2.5" fill="rgba(255,255,255,0.05)" /><rect x="494" y="26" width="10" height="10" rx="2.5" fill="rgba(255,255,255,0.05)" /><rect x="494" y="39" width="10" height="10" rx="2.5" fill="rgba(255,255,255,0.05)" /><rect x="494" y="52" width="10" height="10" rx="2.5" fill="rgba(255,255,255,0.05)" /><rect x="494" y="65" width="10" height="10" rx="2.5" fill="rgba(255,255,255,0.05)" /><rect x="494" y="78" width="10" height="10" rx="2.5" fill="rgba(255,255,255,0.05)" /><rect x="507" y="0" width="10" height="10" rx="2.5" fill="rgba(255,255,255,0.05)" /><rect x="507" y="13" width="10" height="10" rx="2.5" fill="rgba(255,255,255,0.05)" /><rect x="507" y="26" width="10" height="10" rx="2.5" fill="rgba(255,255,255,0.05)" /><rect x="507" y="39" width="10" height="10" rx="2.5" fill="rgba(255,255,255,0.05)" /><rect x="507" y="52" width="10" height="10" rx="2.5" fill="rgba(255,255,255,0.05)" /><rect x="507" y="65" width="10" height="10" rx="2.5" fill="rgba(255,255,255,0.05)" /><rect x="507" y="78" width="10" height="10" rx="2.5" fill="rgba(255,255,255,0.05)" /><rect x="520" y="0" width="10" height="10" rx="2.5" fill="rgba(108,195,130,0.8)" /><rect x="520" y="13" width="10" height="10" rx="2.5" fill="rgba(255,255,255,0.05)" /><rect x="520" y="26" width="10" height="10" rx="2.5" fill="rgba(255,255,255,0.05)" /><rect x="520" y="39" width="10" height="10" rx="2.5" fill="rgba(255,255,255,0.05)" /><rect x="520" y="52" width="10" height="10" rx="2.5" fill="rgba(255,255,255,0.05)" /><rect x="520" y="65" width="10" height="10" rx="2.5" fill="rgba(255,255,255,0.05)" /><rect x="520" y="78" width="10" height="10" rx="2.5" fill="rgba(108,195,130,0.35)" /><rect x="533" y="0" width="10" height="10" rx="2.5" fill="rgba(255,255,255,0.05)" /><rect x="533" y="13" width="10" height="10" rx="2.5" fill="rgba(255,255,255,0.05)" /><rect x="533" y="26" width="10" height="10" rx="2.5" fill="rgba(255,255,255,0.05)" /><rect x="533" y="39" width="10" height="10" rx="2.5" fill="rgba(108,195,130,0.35)" /><rect x="533" y="52" width="10" height="10" rx="2.5" fill="rgba(255,255,255,0.05)" /><rect x="533" y="65" width="10" height="10" rx="2.5" fill="rgba(255,255,255,0.05)" /><rect x="533" y="78" width="10" height="10" rx="2.5" fill="rgba(255,255,255,0.05)" /><rect x="546" y="0" width="10" height="10" rx="2.5" fill="rgba(255,255,255,0.05)" /><rect x="546" y="13" width="10" height="10" rx="2.5" fill="rgba(108,195,130,0.35)" /><rect x="546" y="26" width="10" height="10" rx="2.5" fill="rgba(255,255,255,0.05)" /><rect x="546" y="39" width="10" height="10" rx="2.5" fill="rgba(255,255,255,0.05)" /><rect x="546" y="52" width="10" height="10" rx="2.5" fill="rgba(255,255,255,0.05)" /><rect x="546" y="65" width="10" height="10" rx="2.5" fill="rgba(255,255,255,0.05)" /><rect x="546" y="78" width="10" height="10" rx="2.5" fill="rgba(255,255,255,0.05)" /><rect x="559" y="0" width="10" height="10" rx="2.5" fill="rgba(255,255,255,0.05)" /><rect x="559" y="13" width="10" height="10" rx="2.5" fill="rgba(255,255,255,0.05)" /><rect x="559" y="26" width="10" height="10" rx="2.5" fill="rgba(255,255,255,0.05)" /><rect x="559" y="39" width="10" height="10" rx="2.5" fill="rgba(255,255,255,0.05)" /><rect x="559" y="52" width="10" height="10" rx="2.5" fill="rgba(255,255,255,0.05)" /><rect x="559" y="65" width="10" height="10" rx="2.5" fill="rgba(255,255,255,0.05)" /><rect x="559" y="78" width="10" height="10" rx="2.5" fill="rgba(255,255,255,0.05)" /><rect x="572" y="0" width="10" height="10" rx="2.5" fill="rgba(255,255,255,0.05)" /><rect x="572" y="13" width="10" height="10" rx="2.5" fill="rgba(255,255,255,0.05)" /><rect x="572" y="26" width="10" height="10" rx="2.5" fill="rgba(255,255,255,0.05)" /><rect x="572" y="39" width="10" height="10" rx="2.5" fill="rgba(255,255,255,0.05)" /><rect x="572" y="52" width="10" height="10" rx="2.5" fill="rgba(255,255,255,0.05)" /><rect x="572" y="65" width="10" height="10" rx="2.5" fill="rgba(255,255,255,0.05)" /><rect x="572" y="78" width="10" height="10" rx="2.5" fill="rgba(255,255,255,0.05)" /><rect x="585" y="0" width="10" height="10" rx="2.5" fill="rgba(255,255,255,0.05)" /><rect x="585" y="13" width="10" height="10" rx="2.5" fill="rgba(255,255,255,0.05)" /><rect x="585" y="26" width="10" height="10" rx="2.5" fill="rgba(255,255,255,0.05)" /><rect x="585" y="39" width="10" height="10" rx="2.5" fill="rgba(255,255,255,0.05)" /><rect x="585" y="52" width="10" height="10" rx="2.5" fill="rgba(255,255,255,0.05)" /><rect x="585" y="65" width="10" height="10" rx="2.5" fill="rgba(255,255,255,0.05)" /><rect x="585" y="78" width="10" height="10" rx="2.5" fill="rgba(255,255,255,0.05)" /><rect x="598" y="0" width="10" height="10" rx="2.5" fill="rgba(255,255,255,0.05)" /><rect x="598" y="13" width="10" height="10" rx="2.5" fill="rgba(255,255,255,0.05)" /><rect x="598" y="26" width="10" height="10" rx="2.5" fill="rgba(255,255,255,0.05)" /><rect x="598" y="39" width="10" height="10" rx="2.5" fill="rgba(255,255,255,0.05)" /><rect x="598" y="52" width="10" height="10" rx="2.5" fill="rgba(255,255,255,0.05)" /><rect x="598" y="65" width="10" height="10" rx="2.5" fill="rgba(255,255,255,0.05)" /><rect x="598" y="78" width="10" height="10" rx="2.5" fill="rgba(255,255,255,0.05)" /><rect x="611" y="0" width="10" height="10" rx="2.5" fill="rgba(255,255,255,0.05)" /><rect x="611" y="13" width="10" height="10" rx="2.5" fill="rgba(255,255,255,0.05)" /><rect x="611" y="26" width="10" height="10" rx="2.5" fill="rgba(255,255,255,0.05)" /><rect x="611" y="39" width="10" height="10" rx="2.5" fill="rgba(255,255,255,0.05)" /><rect x="611" y="52" width="10" height="10" rx="2.5" fill="rgba(255,255,255,0.05)" /><rect x="611" y="65" width="10" height="10" rx="2.5" fill="rgba(255,255,255,0.05)" /><rect x="611" y="78" width="10" height="10" rx="2.5" fill="rgba(255,255,255,0.05)" /><rect x="624" y="0" width="10" height="10" rx="2.5" fill="rgba(255,255,255,0.05)" /><rect x="624" y="13" width="10" height="10" rx="2.5" fill="rgba(255,255,255,0.05)" /><rect x="624" y="26" width="10" height="10" rx="2.5" fill="rgba(255,255,255,0.05)" /><rect x="624" y="39" width="10" height="10" rx="2.5" fill="rgba(255,255,255,0.05)" /><rect x="624" y="52" width="10" height="10" rx="2.5" fill="rgba(255,255,255,0.05)" /><rect x="624" y="65" width="10" height="10" rx="2.5" fill="rgba(255,255,255,0.05)" /><rect x="624" y="78" width="10" height="10" rx="2.5" fill="rgba(255,255,255,0.05)" /><rect x="637" y="0" width="10" height="10" rx="2.5" fill="rgba(255,255,255,0.05)" /><rect x="637" y="13" width="10" height="10" rx="2.5" fill="rgba(255,255,255,0.05)" /><rect x="637" y="26" width="10" height="10" rx="2.5" fill="rgba(255,255,255,0.05)" /><rect x="637" y="39" width="10" height="10" rx="2.5" fill="rgba(108,195,130,0.35)" /><rect x="637" y="52" width="10" height="10" rx="2.5" fill="rgba(255,255,255,0.05)" /><rect x="637" y="65" width="10" height="10" rx="2.5" fill="rgba(255,255,255,0.05)" /><rect x="637" y="78" width="10" height="10" rx="2.5" fill="rgba(255,255,255,0.05)" /><rect x="650" y="0" width="10" height="10" rx="2.5" fill="rgba(255,255,255,0.05)" /><rect x="650" y="13" width="10" height="10" rx="2.5" fill="rgba(255,255,255,0.05)" /><rect x="650" y="26" width="10" height="10" rx="2.5" fill="rgba(255,255,255,0.05)" /><rect x="650" y="39" width="10" height="10" rx="2.5" fill="rgba(255,255,255,0.05)" /><rect x="650" y="52" width="10" height="10" rx="2.5" fill="rgba(255,255,255,0.05)" /><rect x="650" y="65" width="10" height="10" rx="2.5" fill="rgba(255,255,255,0.05)" /><rect x="650" y="78" width="10" height="10" rx="2.5" fill="rgba(255,255,255,0.05)" /><rect x="663" y="0" width="10" height="10" rx="2.5" fill="rgba(255,255,255,0.05)" /><rect x="663" y="13" width="10" height="10" rx="2.5" fill="rgba(255,255,255,0.05)" /><rect x="663" y="26" width="10" height="10" rx="2.5" fill="rgba(255,255,255,0.05)" /><rect x="663" y="39" width="10" height="10" rx="2.5" fill="rgba(255,255,255,0.05)" /><rect x="663" y="52" width="10" height="10" rx="2.5" fill="rgba(255,255,255,0.05)" /><rect x="663" y="65" width="10" height="10" rx="2.5" fill="rgba(255,255,255,0.05)" /><rect x="663" y="78" width="10" height="10" rx="2.5" fill="rgba(255,255,255,0.05)" /><rect x="676" y="0" width="10" height="10" rx="2.5" fill="rgba(255,255,255,0.05)" /><rect x="676" y="13" width="10" height="10" rx="2.5" fill="rgba(255,255,255,0.05)" /><rect x="676" y="26" width="10" height="10" rx="2.5" fill="rgba(108,195,130,0.55)" />
      <rect id="rt-scan" x="0" y="-2" width="2" height="92" rx="1" fill="rgba(140,230,165,0.9)" />
    </g>
  </svg>
</div>
```

```aura width=800 height=230
<div style={{ position: 'relative', display: 'flex', flexDirection: 'column', alignItems: 'center', justifyContent: 'center', width: '100%', height: '100%', background: '#08080d', borderRadius: 20, overflow: 'hidden', fontFamily: 'Inter, sans-serif' }}>
  <style>{`
    @keyframes stack-orb { 0%, 100% { transform: translate(0,0); opacity: 0.45; } 50% { transform: translate(18px,-14px); opacity: 0.7; } }
    @keyframes stack-orb-b { 0%, 100% { transform: translate(0,0); opacity: 0.4; } 50% { transform: translate(-14px,10px); opacity: 0.65; } }
    @keyframes chip-appear { 0% { opacity: 0; transform: translateY(8px); } 100% { opacity: 1; transform: translateY(0); } }
    #st-o1 { animation: stack-orb 10s ease-in-out infinite; }
    #st-o2 { animation: stack-orb-b 12s ease-in-out infinite 1s; }
    #st-o3 { animation: stack-orb 9s ease-in-out infinite 2.5s; }
    #st-o4 { animation: stack-orb-b 11s ease-in-out infinite 0.5s; }
  `}</style>
  <svg width="800" height="230" style={{ position: 'absolute', top: 0, left: 0 }}>
    <defs>
      <radialGradient id="sg1" cx="50%" cy="50%" r="50%">
        <stop offset="0%" stopColor="rgba(108,195,130,0.4)" />
        <stop offset="100%" stopColor="rgba(108,195,130,0)" />
      </radialGradient>
      <radialGradient id="sg2" cx="50%" cy="50%" r="50%">
        <stop offset="0%" stopColor="rgba(230,100,115,0.35)" />
        <stop offset="100%" stopColor="rgba(230,100,115,0)" />
      </radialGradient>
      <radialGradient id="sg3" cx="50%" cy="50%" r="50%">
        <stop offset="0%" stopColor="rgba(80,160,220,0.3)" />
        <stop offset="100%" stopColor="rgba(80,160,220,0)" />
      </radialGradient>
      <radialGradient id="sg4" cx="50%" cy="50%" r="50%">
        <stop offset="0%" stopColor="rgba(195,155,255,0.3)" />
        <stop offset="100%" stopColor="rgba(195,155,255,0)" />
      </radialGradient>
    </defs>
    <ellipse id="st-o1" cx="80"  cy="160" rx="160" ry="120" fill="url(#sg1)" />
    <ellipse id="st-o2" cx="730" cy="50"  rx="150" ry="120" fill="url(#sg2)" />
    <ellipse id="st-o3" cx="640" cy="170" rx="140" ry="110" fill="url(#sg3)" />
    <ellipse id="st-o4" cx="180" cy="40"  rx="130" ry="100" fill="url(#sg4)" />
  </svg>
  <span style={{ fontSize: 11, color: 'rgba(255,255,255,0.3)', letterSpacing: 4, textTransform: 'uppercase', marginBottom: 20, zIndex: 10 }}>stack</span>
  <div style={{ display: 'flex', flexWrap: 'wrap', gap: 10, justifyContent: 'center', zIndex: 10, maxWidth: 720 }}>
    {['TypeScript', 'JavaScript', 'React', 'Next.js', 'React Native', 'Tailwind CSS', 'HTML5', 'CSS3', 'Bootstrap', 'Java', 'PostgreSQL', 'MySQL', 'Supabase', 'Figma', 'Photoshop', 'Illustrator', 'Premiere Pro', 'After Effects', 'CapCut'].map((tech, i) => (
      <span key={i} style={{ padding: '7px 18px', background: 'rgba(255,255,255,0.04)', color: 'rgba(255,255,255,0.65)', borderRadius: 100, fontSize: 12, border: '1px solid rgba(255,255,255,0.08)', letterSpacing: 0.5 }}>{tech}</span>
    ))}
  </div>
</div>
```

```aura width=800 height=120
<div style={{ position: 'relative', display: 'flex', flexDirection: 'column', alignItems: 'center', justifyContent: 'center', width: '100%', height: '100%', background: '#08080d', borderRadius: 20, overflow: 'hidden', fontFamily: 'Inter, sans-serif' }}>
  <style>{`
    @keyframes ctfa { 0%, 100% { transform: translate(0,0); opacity: 0.55; } 50% { transform: translate(20px,-14px); opacity: 0.85; } }
    @keyframes ctfb { 0%, 100% { transform: translate(0,0); opacity: 0.45; } 50% { transform: translate(-16px,12px); opacity: 0.75; } }
    #cto1 { animation: ctfa 10s ease-in-out infinite; }
    #cto2 { animation: ctfb 12s ease-in-out infinite 1s; }
    #cto3 { animation: ctfa 9s ease-in-out infinite 2.5s; }
    #cto4 { animation: ctfb 11s ease-in-out infinite 0.5s; }
  `}</style>
  <svg width="800" height="120" style={{ position: 'absolute', top: 0, left: 0 }}>
    <defs>
      <radialGradient id="ctg1" cx="50%" cy="50%" r="50%"><stop offset="0%" stopColor="rgba(108,195,130,0.45)" /><stop offset="100%" stopColor="rgba(108,195,130,0)" /></radialGradient>
      <radialGradient id="ctg2" cx="50%" cy="50%" r="50%"><stop offset="0%" stopColor="rgba(230,100,115,0.4)" /><stop offset="100%" stopColor="rgba(230,100,115,0)" /></radialGradient>
      <radialGradient id="ctg3" cx="50%" cy="50%" r="50%"><stop offset="0%" stopColor="rgba(80,160,220,0.35)" /><stop offset="100%" stopColor="rgba(80,160,220,0)" /></radialGradient>
      <radialGradient id="ctg4" cx="50%" cy="50%" r="50%"><stop offset="0%" stopColor="rgba(195,155,255,0.3)" /><stop offset="100%" stopColor="rgba(195,155,255,0)" /></radialGradient>
    </defs>
    <ellipse id="cto1" cx="120" cy="110" rx="200" ry="150" fill="url(#ctg1)" />
    <ellipse id="cto2" cx="680" cy="10" rx="190" ry="150" fill="url(#ctg2)" />
    <ellipse id="cto3" cx="560" cy="120" rx="180" ry="140" fill="url(#ctg3)" />
    <ellipse id="cto4" cx="260" cy="0" rx="160" ry="120" fill="url(#ctg4)" />
  </svg>
  <span style={{ fontSize: 11, color: 'rgba(255,255,255,0.35)', letterSpacing: 4, textTransform: 'uppercase' }}>vamos conversar</span>
  <span style={{ fontSize: 20, fontWeight: 600, color: '#ffffff', marginTop: 8 }}>Tem um projeto em mente? Me chama.</span>
</div>
```

```aura width=190 height=44 link="https://visionstds.com.br" inline align=center
<SocialMediaButton
  icon="data:image/svg+xml;base64,PHN2ZwogIGNsYXNzPSJsdWNpZGUgbHVjaWRlLWdsb2JlIgogIHhtbG5zPSJodHRwOi8vd3d3LnczLm9yZy8yMDAwL3N2ZyIKICB3aWR0aD0iMjQiCiAgaGVpZ2h0PSIyNCIKICB2aWV3Qm94PSIwIDAgMjQgMjQiCiAgZmlsbD0ibm9uZSIKICBzdHJva2U9IiNmZmZmZmYiCiAgc3Ryb2tlLXdpZHRoPSIyIgogIHN0cm9rZS1saW5lY2FwPSJyb3VuZCIKICBzdHJva2UtbGluZWpvaW49InJvdW5kIgo+CiAgPGNpcmNsZSBjeD0iMTIiIGN5PSIxMiIgcj0iMTAiIC8+CiAgPHBhdGggZD0iTTEyIDJhMTQuNSAxNC41IDAgMCAwIDAgMjAgMTQuNSAxNC41IDAgMCAwIDAtMjAiIC8+CiAgPHBhdGggZD0iTTIgMTJoMjAiIC8+Cjwvc3ZnPg=="
  text="visionstds.com.br"
  backgroundColor="#1a1030"
  width={190}
  height={44}
  gradientStops={[
    { offset: '0%', color: '#ffffff' },
    { offset: '10%', color: '#111111' },
    { offset: '50%', color: '#eeeeee' },
    { offset: '60%', color: '#c39bff' },
    { offset: '80%', color: '#111111' },
    { offset: '100%', color: '#555555' },
  ]}
/>
```

```aura width=120 height=44 link="https://github.com/webdevpls" inline align=center
<SocialMediaButton
  icon="https://cdn.simpleicons.org/github/ffffff"
  text="GitHub"
  backgroundColor="#141414"
  width={120}
  height={44}
  gradientStops={[
    { offset: '0%', color: '#ffffff' },
    { offset: '10%', color: '#111111' },
    { offset: '50%', color: '#eeeeee' },
    { offset: '60%', color: '#ffffff' },
    { offset: '80%', color: '#111111' },
    { offset: '100%', color: '#555555' },
  ]}
/>
```

```aura width=140 height=44 link="https://instagram.com/devpls" inline align=center
<SocialMediaButton
  icon="https://cdn.simpleicons.org/instagram/E4405F"
  text="Instagram"
  backgroundColor="#2b0a17"
  width={140}
  height={44}
  gradientStops={[
    { offset: '0%', color: '#ffffff' },
    { offset: '10%', color: '#111111' },
    { offset: '50%', color: '#eeeeee' },
    { offset: '60%', color: '#E4405F' },
    { offset: '80%', color: '#111111' },
    { offset: '100%', color: '#555555' },
  ]}
/>
```

```aura width=130 height=44 link="https://www.linkedin.com/in/plsnobrega/" inline align=center
<SocialMediaButton
  icon="data:image/svg+xml;base64,PHN2ZyBmaWxsPSIjZmZmZmZmIiByb2xlPSJpbWciIHZpZXdCb3g9IjAgMCAyNCAyNCIgeG1sbnM9Imh0dHA6Ly93d3cudzMub3JnLzIwMDAvc3ZnIj48dGl0bGU+TGlua2VkSW48L3RpdGxlPjxwYXRoIGQ9Ik0yMC40NDcgMjAuNDUyaC0zLjU1NHYtNS41NjljMC0xLjMyOC0uMDI3LTMuMDM3LTEuODUyLTMuMDM3LTEuODUzIDAtMi4xMzYgMS40NDUtMi4xMzYgMi45Mzl2NS42NjdIOS4zNTFWOWgzLjQxNHYxLjU2MWguMDQ2Yy40NzctLjkgMS42MzctMS44NSAzLjM3LTEuODUgMy42MDEgMCA0LjI2NyAyLjM3IDQuMjY3IDUuNDU1djYuMjg2ek01LjMzNyA3LjQzM2MtMS4xNDQgMC0yLjA2My0uOTI2LTIuMDYzLTIuMDY1IDAtMS4xMzguOTItMi4wNjMgMi4wNjMtMi4wNjMgMS4xNCAwIDIuMDY0LjkyNSAyLjA2NCAyLjA2MyAwIDEuMTM5LS45MjUgMi4wNjUtMi4wNjQgMi4wNjV6bTEuNzgyIDEzLjAxOUgzLjU1NVY5aDMuNTY0djExLjQ1MnpNMjIuMjI1IDBIMS43NzFDLjc5MiAwIDAgLjc3NCAwIDEuNzI5djIwLjU0MkMwIDIzLjIyNy43OTIgMjQgMS43NzEgMjRoMjAuNDUxQzIzLjIgMjQgMjQgMjMuMjI3IDI0IDIyLjI3MVYxLjcyOUMyNCAuNzc0IDIzLjIgMCAyMi4yMjIgMGguMDAzeiIvPjwvc3ZnPg=="
  text="LinkedIn"
  backgroundColor="#0a1f33"
  width={130}
  height={44}
  gradientStops={[
    { offset: '0%', color: '#ffffff' },
    { offset: '10%', color: '#111111' },
    { offset: '50%', color: '#eeeeee' },
    { offset: '60%', color: '#0A66C2' },
    { offset: '80%', color: '#111111' },
    { offset: '100%', color: '#555555' },
  ]}
/>
```
