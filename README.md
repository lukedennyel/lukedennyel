<div align="center">

<!-- Animated Header Banner -->
<img src="https://capsule-render.vercel.app/api?type=waving&color=0:0d1117,50:1a1a2e,100:FF2140&height=220&section=header&text=Luke%20Dennyel&fontSize=62&fontColor=ffffff&fontAlignY=35&desc=Game%20Tooling%20%E2%80%A2%20Reverse%20Engineering%20%E2%80%A2%20Modding&descSize=18&descAlignY=55&descAlign=50&animation=fadeIn" width="100%" />

<!-- Typing SVG -->
<a href="https://git.io/typing-svg">
  <img src="https://readme-typing-svg.demolab.com?font=JetBrains+Mono&weight=600&size=22&duration=3000&pause=1000&color=FF2140&center=true&vCenter=true&multiline=false&repeat=true&width=700&height=45&lines=Creator+of+CrewCore+%E2%80%94+%231+Among+Us+Mod+Ecosystem;CurseForge+Top+5+%E2%80%94+32%2B+Stars+%7C+16%2B+Forks;BepInEx+IL2CPP+%2B+Server-Side+Bytecode+VM;Real-Time+WebSocket+%2B+RSA-PSS+Signed+Pipeline;5%2B+Years+Building+Among+Us+Tools" alt="Typing SVG" />
</a>

<br/>

<!-- Social Badges -->
<a href="https://crewcore.online" target="_blank">
  <img src="https://img.shields.io/badge/crewcore.online-FF2140?style=for-the-badge&logo=googlechrome&logoColor=white" height="30" alt="Website" />
</a>
&nbsp;
<a href="https://discord.gg/crewcore" target="_blank">
  <img src="https://img.shields.io/badge/Discord_Server-5865F2?style=for-the-badge&logo=discord&logoColor=white" height="30" alt="Discord" />
</a>
&nbsp;
<a href="https://www.curseforge.com/among-us/all-mods/modmenucrew" target="_blank">
  <img src="https://img.shields.io/badge/CurseForge-Top_5-F16436?style=for-the-badge&logo=curseforge&logoColor=white" height="30" alt="CurseForge" />
</a>

<br/><br/>

<!-- Dynamic Badges -->
<img src="https://img.shields.io/github/stars/MRLuke956/ModMenuCrew?style=for-the-badge&logo=github&logoColor=white&label=ModMenuCrew%20Stars&color=FF2140" alt="Stars" />
&nbsp;
<img src="https://img.shields.io/github/forks/MRLuke956/ModMenuCrew?style=for-the-badge&logo=github&logoColor=white&label=Forks&color=1a1a2e" alt="Forks" />
&nbsp;
<img src="https://img.shields.io/github/license/MRLuke956/ModMenuCrew?style=for-the-badge&color=1a1a2e" alt="License" />

<br/><br/>

<img src="https://komarev.com/ghpvc/?username=MRLuke956&style=for-the-badge&color=FF2140&label=PROFILE+VIEWS" alt="Profile Views" />

</div>

---

### About Me

```yaml
name: Luke Dennyel
location: Brazil
role: Independent Software Developer
focus: Game modding, reverse engineering, real-time systems
building: CrewCore — full-stack Among Us mod ecosystem (since 2025)
stack: C#/.NET (BepInEx IL2CPP) | Node.js (WebSocket + Crypto) | Python | HTML/CSS/JS
achievements: CurseForge Top 5 frontpage | Starstruck badge | 5+ years in Among Us modding
```

I'm the creator of **[CrewCore](https://crewcore.online)**, the **#1 Among Us mod** ranked [Top 5 on CurseForge](https://www.curseforge.com/among-us/all-mods/modmenucrew) — a full-stack ecosystem with **80+ features** spanning a C# BepInEx IL2CPP plugin, a Node.js real-time backend, a web platform with Stripe-powered key system, and a Python Discord bot.

What makes CrewCore different from other mods: the entire UI is **compiled server-side into signed bytecode**, streamed via WebSocket, and executed client-side by a custom IMGUI virtual machine. This means UI updates ship instantly without any client-side patches — a production architecture rarely seen in game modding.

**My journey:** Started with [CrewMod](https://github.com/MRLuke956/CrewMod) in 2021 as a small Among Us mod, evolved into the full CrewCore ecosystem by 2023, and now maintain one of the most feature-rich Among Us modding platforms available.

---

### Architecture

> How CrewCore's server-side bytecode UI pipeline works:

```mermaid
graph LR
    A["C# Client<br/>(BepInEx IL2CPP)"] -- "WebSocket :9223" --> B["Node.js Server"]
    B -- "7 Tab Compilers" --> C["GhostCompiler<br/>Bytecode Assembler"]
    C -- "RSA-PSS Sign<br/>Worker Pool" --> D["POL5 Encrypted<br/>Payload"]
    D -- "Stream" --> A
    A -- "VM Execute<br/>Opcodes" --> E["IMGUI<br/>Renderer"]
    A -- "HTTP :9222" --> F["Web Radar<br/>(Embedded)"]
    style A fill:#1a1a2e,stroke:#FF2140,color:#fff
    style B fill:#1a1a2e,stroke:#FF2140,color:#fff
    style C fill:#1a1a2e,stroke:#FF2140,color:#fff
    style D fill:#1a1a2e,stroke:#FF2140,color:#fff
    style E fill:#1a1a2e,stroke:#FF2140,color:#fff
    style F fill:#1a1a2e,stroke:#FF2140,color:#fff
```

<details>
<summary><b>POL5 Wire Format</b></summary>

```
[MAGIC "POL5" 4B][RSA_SIGNATURE 256B][SESSION_TOKEN 8B][INVERSE_MAP 256B][SEED 4B][TIMESTAMP 8B][SCRAMBLED_BYTECODE...]
```

Every UI frame is cryptographically signed and scrambled before transmission. The client VM descrambles and executes opcodes to render the full mod menu interface.
</details>

---

### Tech Stack

<div align="center">
  <img src="https://skillicons.dev/icons?i=cs,dotnet,nodejs,js,python,html,css,git,github,vscode,visualstudio&theme=dark" alt="Tech Stack" />
</div>

<div align="center">
  <br/>

  ![C#](https://img.shields.io/badge/C%23-239120?style=flat-square&logo=csharp&logoColor=white)
  ![.NET](https://img.shields.io/badge/.NET-512BD4?style=flat-square&logo=dotnet&logoColor=white)
  ![BepInEx](https://img.shields.io/badge/BepInEx-IL2CPP-FF2140?style=flat-square)
  ![Harmony](https://img.shields.io/badge/Harmony-Patches-blueviolet?style=flat-square)
  ![Node.js](https://img.shields.io/badge/Node.js-339933?style=flat-square&logo=nodedotjs&logoColor=white)
  ![WebSocket](https://img.shields.io/badge/WebSocket-010101?style=flat-square&logo=socketdotio&logoColor=white)
  ![RSA-PSS](https://img.shields.io/badge/RSA--PSS-Crypto-FF2140?style=flat-square)
  ![Python](https://img.shields.io/badge/Python-3776AB?style=flat-square&logo=python&logoColor=white)
  ![Stripe](https://img.shields.io/badge/Stripe-008CDD?style=flat-square&logo=stripe&logoColor=white)
  ![Cloudflare](https://img.shields.io/badge/Cloudflare-F38020?style=flat-square&logo=cloudflare&logoColor=white)
  ![IMGUI](https://img.shields.io/badge/IMGUI-Renderer-FF2140?style=flat-square)
  ![dnlib](https://img.shields.io/badge/dnlib-Analysis-blueviolet?style=flat-square)

</div>

---

### CrewCore Ecosystem

<div align="center">

| Component | Stack | Description |
|:---------:|:-----:|:------------|
| **[ModMenuCrew](https://github.com/MRLuke956/ModMenuCrew)** | C# / BepInEx IL2CPP | 80+ features: ESP, impostor control, teleport, speed, noclip, radar, cosmetics unlock, replay system. Custom bytecode VM + IMGUI rendering. **32+ stars** |
| **Server API** | Node.js / WebSocket | Real-time bytecode compiler (GhostCompiler), RSA-PSS signing via worker thread pool, 7 tab compilers, session management |
| **[crewcore.online](https://crewcore.online)** | HTML / CSS / JS | Product website with key generation system, 6 Stripe subscription plans, Cloudflare CDN, i18n (EN/PT-BR) |
| **Discord Bot** | Python | Community management, announcements, status monitoring for the [CrewCore server](https://discord.gg/crewcore) |
| **[AI Knowledge Extractor](https://github.com/MRLuke956/amongus-ai-knowledge-extractor)** | C# / dnlib | AI-powered Among Us .NET/Unity decompiler — generates LLM-ready datasets from game assemblies |
| **Web Radar** | HTML / CSS / JS | Real-time in-browser radar embedded in the mod, served on port 9222 with live player positions |

</div>

---

### Featured Projects

<div align="center">

  <a href="https://github.com/MRLuke956/ModMenuCrew">
    <img src="https://github-readme-stats.vercel.app/api/pin/?username=MRLuke956&repo=ModMenuCrew&theme=github_dark&hide_border=true&icon_color=FF2140&title_color=FF2140" alt="ModMenuCrew" />
  </a>
  <a href="https://github.com/MRLuke956/amongus-ai-knowledge-extractor">
    <img src="https://github-readme-stats.vercel.app/api/pin/?username=MRLuke956&repo=amongus-ai-knowledge-extractor&theme=github_dark&hide_border=true&icon_color=FF2140&title_color=FF2140" alt="AI Knowledge Extractor" />
  </a>

</div>

<div align="center">

  <a href="https://github.com/MRLuke956/userAmongKey">
    <img src="https://github-readme-stats.vercel.app/api/pin/?username=MRLuke956&repo=userAmongKey&theme=github_dark&hide_border=true&icon_color=FF2140&title_color=FF2140" alt="CrewCore Website" />
  </a>
  <a href="https://github.com/MRLuke956/MRLuke956.github.io">
    <img src="https://github-readme-stats.vercel.app/api/pin/?username=MRLuke956&repo=MRLuke956.github.io&theme=github_dark&hide_border=true&icon_color=FF2140&title_color=FF2140" alt="Portfolio" />
  </a>

</div>

---

### Key Highlights

<div align="center">

| | |
|:--|:--|
| **CurseForge Top 5** | Frontpage of Among Us mods — competing with established projects |
| **80+ Features** | ESP, always impostor, teleport, speed hack, noclip, cosmetics unlock, replay system, web radar |
| **Server-Side UI** | Bytecode VM architecture — UI ships as signed opcodes, not hardcoded client code |
| **Replay System** | Full game replay with animation, cosmetics rendering, 22+ event types, chat panel |
| **Web Radar** | Embedded HTTP server serving real-time player positions in-browser |
| **AI Tooling** | Built a decompiler that turns Among Us assemblies into LLM-ready knowledge bases |
| **Active Since 2021** | From CrewMod (first mod) to a full production ecosystem with Stripe monetization |

</div>

---

### GitHub Stats

<div align="center">

  <picture>
    <source media="(prefers-color-scheme: dark)" srcset="https://github-readme-stats.vercel.app/api?username=MRLuke956&show_icons=true&include_all_commits=true&count_private=true&theme=github_dark&hide_border=true&icon_color=FF2140&title_color=FF2140&rank_icon=github" />
    <source media="(prefers-color-scheme: light)" srcset="https://github-readme-stats.vercel.app/api?username=MRLuke956&show_icons=true&include_all_commits=true&count_private=true&theme=default&hide_border=true&icon_color=FF2140&title_color=FF2140&rank_icon=github" />
    <img height="165" alt="GitHub Stats" />
  </picture>
  &nbsp;
  <picture>
    <source media="(prefers-color-scheme: dark)" srcset="https://github-readme-stats.vercel.app/api/top-langs?username=MRLuke956&layout=compact&langs_count=8&theme=github_dark&hide_border=true&title_color=FF2140" />
    <source media="(prefers-color-scheme: light)" srcset="https://github-readme-stats.vercel.app/api/top-langs?username=MRLuke956&layout=compact&langs_count=8&theme=default&hide_border=true&title_color=FF2140" />
    <img height="165" alt="Top Languages" />
  </picture>

</div>

<div align="center">

  <picture>
    <source media="(prefers-color-scheme: dark)" srcset="https://streak-stats.demolab.com?user=MRLuke956&theme=github-dark&hide_border=true&ring=FF2140&fire=FF2140&currStreakLabel=FF2140" />
    <source media="(prefers-color-scheme: light)" srcset="https://streak-stats.demolab.com?user=MRLuke956&theme=default&hide_border=true&ring=FF2140&fire=FF2140&currStreakLabel=FF2140" />
    <img alt="GitHub Streak" />
  </picture>

</div>

---

### Trophies

<div align="center">
  <img src="https://github-profile-trophy.vercel.app/?username=MRLuke956&theme=darkhub&no-frame=true&no-bg=true&column=7&margin-w=10" alt="Trophies" />
</div>

---

### Contribution Graph

<div align="center">
  <picture>
    <source media="(prefers-color-scheme: dark)" srcset="https://raw.githubusercontent.com/MRLuke956/MRLuke956/output/github-snake-dark.svg" />
    <source media="(prefers-color-scheme: light)" srcset="https://raw.githubusercontent.com/MRLuke956/MRLuke956/output/github-snake.svg" />
    <img alt="Snake animation" width="100%" />
  </picture>
</div>

<!--
  To enable the snake animation, create .github/workflows/snake.yml in your MRLuke956/MRLuke956 repo:
  https://github.com/Platane/snk — generates the SVG daily via GitHub Actions
-->

---

<div align="center">
  <img src="https://capsule-render.vercel.app/api?type=waving&color=0:0d1117,50:1a1a2e,100:FF2140&height=100&section=footer" width="100%" />
</div>
