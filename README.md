<div align="center">

  <img src="./assets/vaultbit-coins-banner.jpg" alt="Daniel Brosed — Blockchain Security Auditor & AI Systems Engineer" width="100%" style="border-radius: 12px; box-shadow: 0 25px 60px rgba(0,0,0,0.85);" />

  <br/><br/>

  <p align="center">
    <code>BLOCKCHAIN SECURITY AUDITOR</code> &nbsp;·&nbsp; 
    <code>SOLIDITY ENGINEER</code> &nbsp;·&nbsp; 
    <code>AI SYSTEMS ARCHITECT</code>
  </p>

  <p align="center">
    <a href="https://profiles.cyfrin.io/u/danielbrosed"><img src="https://img.shields.io/badge/Cyfrin_Security-Updraft_Verified-3ECF8E?style=for-the-badge&logo=ethereum&logoColor=0A0A0A" alt="Cyfrin Updraft" /></a>
    <a href="https://danielbrosed.com"><img src="https://img.shields.io/badge/danielbrosed.com-Official_Site-FC8323?style=for-the-badge&logo=astro&logoColor=0A0A0A" alt="Website" /></a>
    <a href="https://linkedin.com/in/danielbrosed"><img src="https://img.shields.io/badge/LinkedIn-Connect-6E99FF?style=for-the-badge&logo=linkedin&logoColor=0A0A0A" alt="LinkedIn" /></a>
    <a href="https://t.me/danielbrosed"><img src="https://img.shields.io/badge/Telegram-Encrypted-FC8323?style=for-the-badge&logo=telegram&logoColor=0A0A0A" alt="Telegram" /></a>
  </p>

  <br/>

  <p align="center">
    <em>"Audito la lógica económica, la seguridad criptográfica y los vectores de ataque en smart contracts antes de que cuesten millones en TVL. Especializado en suites de testing con Foundry, análisis estático y protocolos de custodia física en VaultBit."</em>
  </p>

</div>

<br/>

---

### 🛡️ Core de Auditoría · Vectores y Metodología en Smart Contracts

Mi trabajo de auditoría en Web3 se apoya en análisis formal, invariant testing basado en propiedades y verificación de vectores de exploit críticos en EVM:

```
┌────────────────────────────────────────────────────────────────────────────────────────┐
│                              SECURITY AUDIT TAXONOMY                                   │
├────────────────────────────┬─────────────────────────────┬─────────────────────────────┤
│ 01 · LÓGICA Y CONTROL      │ 02 · ORÁCULOS Y DEFI        │ 03 · CRIPTOGRAFÍA Y KEYS    │
│ • Reentrancy (Cross/Read)  │ • Spot vs TWAP Manipulation │ • EIP-712 Signature Replay  │
│ • State Machine Invariants │ • Flash Loan Arbitrage      │ • BIP-39 Key Derivation     │
│ • Access Control / Proxies │ • Rounding & Precision Loss │ • ERC-4337 Account Abstr.   │
│ • Unchecked Return Values  │ • Slippage & Sandwich Risks │ • Multisig / Safe Guards    │
└────────────────────────────┴─────────────────────────────┴─────────────────────────────┘
```

#### 🔬 Toolchain de Auditoría y Verificación:
- **Foundry (`forge`, `cast`, `anvil`)**: Testing basado en propiedades (fuzzing con miles de runs), invariant testing diferencial y forking de mainnet con RPCs de alta concurrencia.
- **Análisis Estático & Simbólico**: `Slither` (detectores custom de AST), `Aderyn`, `Echidna` y `Medusa` para cobertura de estados extremos.
- **Estándares y Checklists**: OWASP Smart Contract Top 10, SWC Registry, Secureum mindmaps y reportes de investigación de CodeHawks / Solodit.

```solidity
// PoC: Invariant Test Harness (Foundry)
function invariant_ProtocolSolvencyMaintained() public view {
    uint256 totalDeposited = vault.totalAssets();
    uint256 totalTrackedShares = vault.totalSupply();
    assertGe(totalDeposited, totalTrackedShares, "CRITICAL: Solvency broken by precision loss");
}
```

<br/>

---

### 🏆 Credenciales de Seguridad · Cyfrin Updraft

Formación exhaustiva y exámenes completados en la academia de seguridad Web3 coliderada por Patrick Collins:

| Credencial Cyfrin Updraft | Estado | Alcance Técnico Auditado |
|:---|:---:|:---|
| **Smart Contract Security & Auditing** | [Verificar ↗](https://profiles.cyfrin.io/u/danielbrosed/achievements/smart-contract-security-and-auditing) | Vectores de reentrancy profunda, manipulación de oráculos, control de acceso, fuzzing diferencial en Foundry y redacción de informes con severidad High/Medium/Low. |
| **Solidity Smart Contract Development** | [Verificar ↗](https://profiles.cyfrin.io/u/danielbrosed/achievements/solidity-smart-contract-development) | Patrones de arquitectura EVM, layout de storage/memory, gas optimization avanzado, herencia múltiple y estándares ERC-20, ERC-721, ERC-1155, ERC-4626. |
| **Advanced Web3 Wallet Security** | [Verificar ↗](https://profiles.cyfrin.io/u/danielbrosed/achievements/advanced-web3-wallet-security) | Permisos y aprobaciones ERC-20 (`permit`), Account Abstraction (ERC-4337), esquemas multi-firma con Safe y aislamiento de tesorería institucional. |
| **Web3 Wallet Security Basics** | [Verificar ↗](https://profiles.cyfrin.io/u/danielbrosed/achievements/web3-wallet-security-basics) | Arquitectura de claves privadas BIP-39, derivación jerárquica, transacciones sin procesar, firmas de curvas elípticas (secp256k1) y mitigación de phishing. |
| **Blockchain Basics** | [Verificar ↗](https://profiles.cyfrin.io/u/danielbrosed/achievements/blockchain-basics) | Hashes criptográficos SHA-256/Keccak-256, estructura de bloques, mempools, consenso descentralizado y ejecución determinista en EVM. |

<br/>

---

### 🏛️ Proyectos Web3 e Infraestructura Criptográfica

<table align="center" width="100%" border="0" cellpadding="0" cellspacing="0">
  <tr>
    <td width="33%" valign="top">
      <a href="https://vaultbit.es"><img src="./assets/brands/vaultbit-white.png" height="32" alt="VaultBit" /></a><br/>
      <strong>VaultBit</strong><br/>
      <sub>Infraestructura física de custodia en frío (cold storage redundante) y protocolo descentralizado de herencia para Bitcoin y activos de alto patrimonio.</sub>
    </td>
    <td width="33%" valign="top">
      <img src="./assets/brands/inheritance-horizontal-negativo.png" height="28" alt="Inheritance Protocol" /><br/>
      <strong>Protocolo de Herencia</strong><br/>
      <sub>Arquitectura criptográfica sin intermediarios para asegurar la transferencia no custodial de patrimonio digital mediante esquemas multi-clave y timelocks.</sub>
    </td>
    <td width="33%" valign="top">
      <strong>Sole Hand / FeeSplitter</strong><br/>
      <sub>Smart contracts Solidity en producción para liquidación automatizada y reparto programable de cobros con account abstraction en redes EVM.</sub>
    </td>
  </tr>
  <tr>
    <td width="33%" valign="top">
      <br/>
      <a href="https://vaultbit.es/vaultgrid"><img src="./assets/brands/vaultgrid-white.png" height="28" alt="VaultGrid Labs" /></a><br/>
      <strong>VaultGrid Labs</strong><br/>
      <sub>Sistemas de almacenamiento de energía con baterías (BESS) para naves industriales y renovables: la infraestructura física que sostendrá la computación y la IA.</sub>
    </td>
    <td width="33%" valign="top">
      <br/>
      <a href="https://balority.app"><img src="./assets/brands/balority.svg" height="26" alt="Balority" /></a><br/>
      <strong>Balority App</strong><br/>
      <sub>Auditoría de seguridad con metodología OWASP: 29 hallazgos identificados (5 de severidad crítica/grave) y motor de conexiones con IA.</sub>
    </td>
    <td width="33%" valign="top">
      <br/>
      <a href="https://ceseagencia.com"><img src="./assets/brands/cesea-white.png" height="26" alt="Cesea" /></a><br/>
      <strong>Cesea Agenc.ia</strong><br/>
      <sub>Automatización de prospección comercial con agentes de IA: reducción del tiempo de cualificación de 3 h 04 min a 5 min.</sub>
    </td>
  </tr>
</table>

<br/>

---

### 🧠 Inteligencia Artificial como Multiplicador de Auditoría

No utilizo la IA como un sustituto del criterio humano, sino como un **motor acelerador de análisis formal y generación de tests**:

- **Anthropic Academy Certified**: 10 certificaciones oficiales de Anthropic (creadora de Claude), incluyendo *Claude Code in Action*, *Introduction to Agent Skills*, *AI Fluency for Builders*, y *Model Context Protocol (MCP)*.
- **Herramientas de Auditoría Asistidas**: Agentes autónomos para análisis sintáctico de AST, barrido diferencial de contratos y síntesis automática de arneses de prueba en Foundry.
- **Orquestación de Pipelines**: Integración de flujos de análisis con n8n, bases de datos vectoriales en Supabase pgvector y modelos frontera Claude 3.5 Sonnet.

<br/>

---

### 💻 Stack Tecnológico

<div align="center">

<p align="center">
  <img src="https://img.shields.io/badge/Solidity-0A0A0A?style=for-the-badge&logo=solidity&logoColor=AA6746" />
  <img src="https://img.shields.io/badge/Foundry-0A0A0A?style=for-the-badge&logo=ethereum&logoColor=3ECF8E" />
  <img src="https://img.shields.io/badge/Slither-0A0A0A?style=for-the-badge&logo=security&logoColor=FC8323" />
  <img src="https://img.shields.io/badge/Ethereum-0A0A0A?style=for-the-badge&logo=ethereum&logoColor=6E99FF" />
  <img src="https://img.shields.io/badge/Bitcoin_Cold_Storage-0A0A0A?style=for-the-badge&logo=bitcoin&logoColor=FC8323" />
  <img src="https://img.shields.io/badge/TypeScript-0A0A0A?style=for-the-badge&logo=typescript&logoColor=3178C6" />
  <img src="https://img.shields.io/badge/Python-0A0A0A?style=for-the-badge&logo=python&logoColor=3776AB" />
  <img src="https://img.shields.io/badge/Anthropic_Claude-0A0A0A?style=for-the-badge&logo=anthropic&logoColor=FC8323" />
</p>

<p align="center">
  <a href="https://skillicons.dev">
    <img src="https://skillicons.dev/icons?i=solidity,ts,python,react,nextjs,astro,tailwind,nodejs,postgres,docker,linux,git&theme=dark" />
  </a>
</p>

</div>

<br/>

---

### 📂 Repositorios de Arquitectura & Seguridad

<table align="center" border="0" width="100%" cellpadding="0" cellspacing="0">
  <tr>
    <td width="50%" align="center">
      <a href="https://github.com/danielbrosed/vaultbit-website">
        <img src="https://github-readme-stats.vercel.app/api/pin/?username=danielbrosed&repo=vaultbit-website&theme=dark&bg_color=0A0A0A&title_color=FC8323&icon_color=FC8323&text_color=F5F4EF&border_color=1F2228" alt="VaultBit Website" width="100%" />
      </a>
    </td>
    <td width="50%" align="center">
      <a href="https://github.com/danielbrosed/vaultbit-ops">
        <img src="https://github-readme-stats.vercel.app/api/pin/?username=danielbrosed&repo=vaultbit-ops&theme=dark&bg_color=0A0A0A&title_color=FC8323&icon_color=FC8323&text_color=F5F4EF&border_color=1F2228" alt="VaultBit Ops" width="100%" />
      </a>
    </td>
  </tr>
  <tr>
    <td width="50%" align="center">
      <a href="https://github.com/danielbrosed/SOLE-HAND-PROYECT">
        <img src="https://github-readme-stats.vercel.app/api/pin/?username=danielbrosed&repo=SOLE-HAND-PROYECT&theme=dark&bg_color=0A0A0A&title_color=FC8323&icon_color=FC8323&text_color=F5F4EF&border_color=1F2228" alt="Sole Hand" width="100%" />
      </a>
    </td>
    <td width="50%" align="center">
      <a href="https://github.com/danielbrosed/cesea-agencia-case-study">
        <img src="https://github-readme-stats.vercel.app/api/pin/?username=danielbrosed&repo=cesea-agencia-case-study&theme=dark&bg_color=0A0A0A&title_color=FC8323&icon_color=FC8323&text_color=F5F4EF&border_color=1F2228" alt="Cesea Agencia" width="100%" />
      </a>
    </td>
  </tr>
</table>

<br/>

<!-- GITHUB STATS & METRICS -->
<div align="center">

<table align="center" border="0" width="100%" cellpadding="0" cellspacing="0">
  <tr>
    <td width="50%" align="center" valign="top">
      <img src="https://github-readme-stats.vercel.app/api?username=danielbrosed&show_icons=true&theme=dark&bg_color=0A0A0A&title_color=FC8323&icon_color=FC8323&text_color=F5F4EF&border_color=1F2228&hide_border=false&count_private=true" alt="GitHub Stats" width="100%" />
    </td>
    <td width="50%" align="center" valign="top">
      <img src="https://github-readme-stats.vercel.app/api/top-langs/?username=danielbrosed&layout=compact&theme=dark&bg_color=0A0A0A&title_color=FC8323&text_color=F5F4EF&border_color=1F2228&hide_border=false&langs_count=6" alt="Top Languages" width="100%" />
    </td>
  </tr>
</table>

<br/>

<img src="https://github-readme-activity-graph.vercel.app/graph?username=danielbrosed&bg_color=0A0A0A&color=FC8323&line=FC8323&point=F5F4EF&area_color=FC8323&area=true&hide_border=false&custom_title=Daniel%20Brosed%20%C2%B7%20Activity&border_color=1F2228" alt="Activity Graph" width="95%" />

<br/><br/>

<img src="https://komarev.com/ghpvc/?username=danielbrosed&style=flat-square&color=FC8323&label=AUDITOR+PROFILE+VIEWS" alt="Profile Views" />

</div>
