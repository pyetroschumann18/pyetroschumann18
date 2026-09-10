<img width="1200" height="400" alt="hero" src="https://github.com/user-attachments/assets/df64bfff-16f2-4da9-b472-4b05efa44b35" />![Uploading hero.sv<svg xmlns="http://www.w3.org/2000/svg" width="1200" height="400" viewBox="0 0 1200 400" role="img" aria-labelledby="title desc">
  <title id="title">Pyetro Schumann — Web Developer</title>
  <desc id="desc">Animated dark purple developer banner with a terminal window, moving lights and code elements.</desc>

  <defs>
    <linearGradient id="background" x1="0" y1="0" x2="1" y2="1">
      <stop offset="0" stop-color="#070A12" />
      <stop offset="0.52" stop-color="#0D1117" />
      <stop offset="1" stop-color="#11101D" />
    </linearGradient>

    <linearGradient id="accent" x1="0" y1="0" x2="1" y2="0">
      <stop offset="0" stop-color="#584EDD" />
      <stop offset="0.5" stop-color="#B27CF4" />
      <stop offset="1" stop-color="#7C5CE7" />
    </linearGradient>

    <linearGradient id="shine" x1="-1" y1="0" x2="0" y2="0">
      <stop offset="0" stop-color="#FFFFFF" stop-opacity="0" />
      <stop offset="0.5" stop-color="#FFFFFF" stop-opacity="0.5" />
      <stop offset="1" stop-color="#FFFFFF" stop-opacity="0" />
    </linearGradient>

    <radialGradient id="glowPurple">
      <stop offset="0" stop-color="#B27CF4" stop-opacity="0.36" />
      <stop offset="1" stop-color="#B27CF4" stop-opacity="0" />
    </radialGradient>

    <pattern id="grid" width="32" height="32" patternUnits="userSpaceOnUse">
      <path d="M 32 0 L 0 0 0 32" fill="none" stroke="#B27CF4" stroke-width="0.7" stroke-opacity="0.08" />
    </pattern>

    <filter id="softGlow" x="-100%" y="-100%" width="300%" height="300%">
      <feGaussianBlur stdDeviation="6" result="blur" />
      <feMerge>
        <feMergeNode in="blur" />
        <feMergeNode in="SourceGraphic" />
      </feMerge>
    </filter>

    <clipPath id="frameClip">
      <rect x="8" y="8" width="1184" height="384" rx="24" />
    </clipPath>

    <clipPath id="terminalClip">
      <rect x="704" y="77" width="416" height="246" rx="16" />
    </clipPath>

    <style>
      .font { font-family: "Segoe UI", Inter, Arial, sans-serif; }
      .mono { font-family: "Cascadia Code", "Fira Code", Consolas, monospace; }

      .float-a { animation: floatA 7s ease-in-out infinite; }
      .float-b { animation: floatB 9s ease-in-out infinite; }
      .pulse { animation: pulse 2.8s ease-in-out infinite; transform-origin: center; }
      .blink { animation: blink 1s steps(2, end) infinite; }
      .code-1 { animation: codeIn 8s ease-in-out infinite; }
      .code-2 { animation: codeIn 8s 0.5s ease-in-out infinite; opacity: 0; }
      .code-3 { animation: codeIn 8s 1s ease-in-out infinite; opacity: 0; }
      .code-4 { animation: codeIn 8s 1.5s ease-in-out infinite; opacity: 0; }
      .code-5 { animation: codeIn 8s 2s ease-in-out infinite; opacity: 0; }
      .scan { animation: scan 5.5s linear infinite; }
      .dash { stroke-dasharray: 12 10; animation: dash 14s linear infinite; }
      .name { animation: nameIn 1.2s cubic-bezier(.2,.8,.2,1) both; }
      .role { animation: nameIn 1.2s .25s cubic-bezier(.2,.8,.2,1) both; }
      .status { animation: nameIn 1.2s .5s cubic-bezier(.2,.8,.2,1) both; }

      @keyframes floatA {
        0%, 100% { transform: translate(0, 0); }
        50% { transform: translate(16px, -12px); }
      }
      @keyframes floatB {
        0%, 100% { transform: translate(0, 0); }
        50% { transform: translate(-18px, 16px); }
      }
      @keyframes pulse {
        0%, 100% { opacity: .55; transform: scale(1); }
        50% { opacity: 1; transform: scale(1.28); }
      }
      @keyframes blink { 50% { opacity: 0; } }
      @keyframes codeIn {
        0%, 5% { opacity: 0; transform: translateX(-12px); }
        15%, 82% { opacity: 1; transform: translateX(0); }
        92%, 100% { opacity: 0; transform: translateX(8px); }
      }
      @keyframes scan {
        0% { transform: translateX(-560px); opacity: 0; }
        12% { opacity: .7; }
        65% { opacity: .35; }
        100% { transform: translateX(1050px); opacity: 0; }
      }
      @keyframes dash { to { stroke-dashoffset: -220; } }
      @keyframes nameIn {
        from { opacity: 0; transform: translateY(18px); }
        to { opacity: 1; transform: translateY(0); }
      }

      @media (prefers-reduced-motion: reduce) {
        * { animation: none !important; }
        .code-2, .code-3, .code-4, .code-5 { opacity: 1; }
      }
    </style>
  </defs>

  <g clip-path="url(#frameClip)">
    <rect width="1200" height="400" fill="url(#background)" />
    <rect width="1200" height="400" fill="url(#grid)" />

    <circle class="float-a" cx="130" cy="82" r="185" fill="url(#glowPurple)" />
    <circle class="float-b" cx="1050" cy="340" r="240" fill="url(#glowPurple)" opacity="0.55" />

    <path class="dash" d="M-10 344 C235 272 337 446 612 342 S1000 260 1220 316" fill="none" stroke="url(#accent)" stroke-width="2" opacity="0.24" />

    <g opacity="0.7">
      <circle class="pulse" cx="94" cy="320" r="3" fill="#B27CF4" filter="url(#softGlow)" />
      <circle class="pulse" cx="1128" cy="70" r="3" fill="#7C5CE7" filter="url(#softGlow)" style="animation-delay:.7s" />
      <circle class="pulse" cx="641" cy="47" r="2.5" fill="#B27CF4" filter="url(#softGlow)" style="animation-delay:1.2s" />
      <circle class="pulse" cx="532" cy="350" r="2.5" fill="#7C5CE7" filter="url(#softGlow)" style="animation-delay:1.8s" />
    </g>

    <g transform="translate(76 90)">
      <g class="status">
        <circle cx="8" cy="10" r="7" fill="#3FB950" opacity="0.2" />
        <circle cx="8" cy="10" r="3.5" fill="#3FB950" />
        <text x="24" y="15" class="mono" fill="#8B949E" font-size="14" letter-spacing="1.2">AVAILABLE TO BUILD</text>
      </g>

      <text x="0" y="92" class="font name" fill="#FFFFFF" font-size="61" font-weight="800" letter-spacing="-1.5">PYETRO</text>
      <text x="0" y="151" class="font name" fill="url(#accent)" font-size="61" font-weight="800" letter-spacing="-1.5">SCHUMANN</text>

      <g class="role">
        <rect x="0" y="183" width="476" height="2" rx="1" fill="url(#accent)" />
        <rect class="scan" x="0" y="180" width="90" height="8" fill="url(#shine)" />
        <text x="0" y="222" class="mono" fill="#C9D1D9" font-size="18" letter-spacing="2.1">WEB DEVELOPER</text>
        <text x="218" y="222" class="mono" fill="#6E7681" font-size="18">/</text>
        <text x="244" y="222" class="mono" fill="#B27CF4" font-size="18" letter-spacing="1.2">DIGITAL PRODUCTS</text>
      </g>
    </g>

    <g clip-path="url(#terminalClip)">
      <rect x="704" y="77" width="416" height="246" rx="16" fill="#0A0D14" stroke="#30363D" />
      <rect x="704" y="77" width="416" height="42" fill="#161B22" />
      <circle cx="729" cy="98" r="5" fill="#FF5F57" />
      <circle cx="747" cy="98" r="5" fill="#FEBC2E" />
      <circle cx="765" cy="98" r="5" fill="#28C840" />
      <text x="810" y="104" class="mono" fill="#6E7681" font-size="12">pyetro.ts</text>

      <g class="mono" font-size="14">
        <g class="code-1">
          <text x="730" y="154" fill="#8B949E">01</text>
          <text x="760" y="154" fill="#FF7B72">const</text>
          <text x="808" y="154" fill="#D2A8FF">developer</text>
          <text x="886" y="154" fill="#C9D1D9">= {</text>
        </g>
        <g class="code-2">
          <text x="730" y="184" fill="#8B949E">02</text>
          <text x="780" y="184" fill="#79C0FF">craft:</text>
          <text x="835" y="184" fill="#A5D6FF">&quot;web&quot;</text>
          <text x="883" y="184" fill="#C9D1D9">,</text>
        </g>
        <g class="code-3">
          <text x="730" y="214" fill="#8B949E">03</text>
          <text x="780" y="214" fill="#79C0FF">mindset:</text>
          <text x="855" y="214" fill="#A5D6FF">&quot;product&quot;</text>
          <text x="930" y="214" fill="#C9D1D9">,</text>
        </g>
        <g class="code-4">
          <text x="730" y="244" fill="#8B949E">04</text>
          <text x="780" y="244" fill="#79C0FF">quality:</text>
          <text x="850" y="244" fill="#A5D6FF">true</text>
          <text x="885" y="244" fill="#C9D1D9">,</text>
        </g>
        <g class="code-5">
          <text x="730" y="274" fill="#8B949E">05</text>
          <text x="760" y="274" fill="#C9D1D9">};</text>
          <text x="730" y="304" fill="#8B949E">06</text>
          <text x="760" y="304" fill="#B27CF4">build</text>
          <text x="800" y="304" fill="#C9D1D9">();</text>
          <rect class="blink" x="836" y="290" width="8" height="18" fill="#B27CF4" />
        </g>
      </g>
    </g>
  </g>

  <rect x="8" y="8" width="1184" height="384" rx="24" fill="none" stroke="url(#accent)" stroke-width="2" opacity="0.72" />
</svg>
g…]()

<!--
  Pyetro Schumann — GitHub Profile README
  Keep the assets/hero.svg file beside this README when publishing.
-->

<div align="center">
  <img
    width="100%"
    src="./assets/hero.svg"
    alt="Animated banner: Pyetro Schumann, Web Developer"
  />
</div>

<div align="center">
  <a href="https://git.io/typing-svg">
    <img
      src="https://readme-typing-svg.demolab.com?font=Fira+Code&weight=600&size=22&duration=2600&pause=850&color=B27CF4&center=true&vCenter=true&repeat=true&random=false&width=820&height=55&lines=Turning+ideas+into+real+digital+products.;Frontend%2C+backend+and+everything+in+between.;Clean+code.+Fast+experiences.+Useful+solutions.;Always+building%2C+testing+and+improving."
      alt="Typing animation introducing Pyetro's work"
    />
  </a>
</div>

<p align="center">
  <a href="https://github.com/pyetroschumann18">
    <img src="https://img.shields.io/badge/GitHub-0D1117?style=for-the-badge&logo=github&logoColor=white" alt="GitHub" />
  </a>
  <img src="https://img.shields.io/badge/Brazil-0D1117?style=for-the-badge&logo=googlemaps&logoColor=B27CF4" alt="Brazil" />
  <img src="https://img.shields.io/badge/Open_to_build-7C5CE7?style=for-the-badge&logo=rocket&logoColor=white" alt="Open to build" />
</p>

<p align="center">
  <strong>Web Developer focused on creating modern, performant and useful products.</strong>
</p>

<br/>

## `> whoami`

```ts
const pyetro = {
  role: "Web Developer",
  location: "Brazil 🇧🇷",

  mission: "Turn business ideas into products people enjoy using.",

  focus: [
    "Frontend Development",
    "Backend Development",
    "Software Architecture",
    "AI-assisted Development"
  ],

  building: ["Afinity-Car", "MOV Digital"],

  values: [
    "Useful over flashy",
    "Clarity over complexity",
    "Performance by default",
    "Build, understand, test, improve"
  ]
} as const;
```

<br/>

## ⚡ Technologies I use

<div align="center">

### Frontend

<img
  src="https://skillicons.dev/icons?i=html,css,js,ts,react,astro,tailwind&theme=dark&perline=7"
  alt="HTML, CSS, JavaScript, TypeScript, React, Astro and Tailwind CSS"
/>

### Backend & Data

<img
  src="https://skillicons.dev/icons?i=nodejs,supabase,postgres&theme=dark&perline=3"
  alt="Node.js, Supabase and PostgreSQL"
/>

### Tools & Workflow

<img
  src="https://skillicons.dev/icons?i=git,github,vscode,vercel,figma&theme=dark&perline=5"
  alt="Git, GitHub, Visual Studio Code, Vercel and Figma"
/>

</div>

<br/>

## 💜 Currently building

<table>
  <tr>
    <td width="50%" valign="top">
      <h3>🚗 Afinity-Car</h3>
      <p>A digital product built around a real use case, combining thoughtful interfaces, reliable data and a smooth user experience.</p>
      <p><strong>Product • Frontend • Backend • UX</strong></p>
    </td>
    <td width="50%" valign="top">
      <h3>🚀 MOV Digital</h3>
      <p>Modern, conversion-focused websites and digital experiences for small businesses and entrepreneurs.</p>
      <p><strong>Web • Automation • Performance • Conversion</strong></p>
    </td>
  </tr>
</table>

At **MOV Digital**, I work across the product cycle: responsive interfaces, frontend and backend structure, UX/UI improvements, databases, automations and deployment.

<br/>

## 🧠 What I am improving now

<p align="center">
  <img src="https://img.shields.io/badge/Software_Architecture-0D1117?style=flat-square&logoColor=white" alt="Software Architecture" />
  <img src="https://img.shields.io/badge/TypeScript-0D1117?style=flat-square&logo=typescript&logoColor=3178C6" alt="TypeScript" />
  <img src="https://img.shields.io/badge/React-0D1117?style=flat-square&logo=react&logoColor=61DAFB" alt="React" />
  <img src="https://img.shields.io/badge/Astro-0D1117?style=flat-square&logo=astro&logoColor=BC52EE" alt="Astro" />
  <img src="https://img.shields.io/badge/PostgreSQL-0D1117?style=flat-square&logo=postgresql&logoColor=4169E1" alt="PostgreSQL" />
  <img src="https://img.shields.io/badge/Testing-0D1117?style=flat-square&logo=vitest&logoColor=6E9F18" alt="Testing" />
  <img src="https://img.shields.io/badge/Security-0D1117?style=flat-square&logo=owasp&logoColor=white" alt="Security" />
  <img src="https://img.shields.io/badge/Performance-0D1117?style=flat-square&logo=lighthouse&logoColor=F44B21" alt="Performance" />
</p>

<br/>

## 📊 GitHub analytics

<div align="center">
  <img
    width="49%"
    src="https://github-profile-summary-cards.vercel.app/api/cards/stats?username=pyetroschumann18&theme=github_dark&title_color=B27CF4&text_color=FFFFFF&bg_color=0D1117&border_color=21262D&icon_color=B27CF4&animation=sequence&duration=3.2"
    alt="Pyetro's GitHub statistics"
  />
  <img
    width="49%"
    src="https://github-profile-summary-cards.vercel.app/api/cards/repos-per-language?username=pyetroschumann18&theme=github_dark&title_color=B27CF4&text_color=FFFFFF&bg_color=0D1117&border_color=21262D&chart_color=B27CF4&animation=draw&duration=3.8"
    alt="Most used languages by repository"
  />
</div>

<div align="center">
  <img
    width="70%"
    src="https://streak-stats.demolab.com?user=pyetroschumann18&background=0D1117&border=21262D&stroke=30363D&ring=B27CF4&fire=7C5CE7&currStreakNum=FFFFFF&sideNums=FFFFFF&currStreakLabel=B27CF4&sideLabels=B27CF4&dates=8B949E&hide_border=false&border_radius=8"
    alt="Pyetro's GitHub contribution streak"
  />
</div>

<br/>

## 📈 Contribution timeline

<div align="center">
  <img
    width="100%"
    src="https://github-profile-summary-cards.vercel.app/api/cards/profile-details?username=pyetroschumann18&theme=github_dark&title_color=B27CF4&text_color=FFFFFF&bg_color=0D1117&border_color=21262D&icon_color=B27CF4&chart_color=7C5CE7&animation=load&duration=4.5"
    alt="Pyetro's GitHub contribution timeline"
  />
</div>

<div align="center">
  <img
    width="100%"
    src="https://github-readme-activity-graph.vercel.app/graph?username=pyetroschumann18&bg_color=0D1117&color=B27CF4&title_color=B27CF4&line=7C5CE7&point=FFFFFF&area_color=7C5CE7&area=true&hide_border=false&border_color=21262D&radius=8&custom_title=Contribution%20Activity"
    alt="Pyetro's recent contribution activity graph"
  />
</div>

<br/>

## 🌎 Let's build something useful

<p align="center">
  I enjoy turning rough ideas into reliable digital experiences.<br/>
  If the project needs clear interfaces, solid structure and attention to detail, I am interested.
</p>

<p align="center">
  <a href="https://github.com/pyetroschumann18">
    <img src="https://img.shields.io/badge/Explore_my_work-B27CF4?style=for-the-badge&logo=github&logoColor=0D1117" alt="Explore Pyetro's work on GitHub" />
  </a>
</p>

<br/>

<div align="center">
  <sub><strong>Build. Understand. Test. Improve.</strong></sub>
</div>

<img
  width="100%"
  src="https://capsule-render.vercel.app/api?type=waving&color=0:584EDD,50:7C5CE7,100:B27CF4&height=110&section=footer"
  alt="Purple gradient footer"
/>
