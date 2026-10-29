# Hyojun Jo (조효준)

> **Systems Architect & AI Tooling Engineer**  
> Architecting deterministic developer tooling, zero-driver network telemetry, and Model Context Protocol (MCP) ecosystems.

---

### 🌐 Language Navigation (10 Languages)

| 🇰🇷 [한국어](#korean) | 🇺🇸 [English](#english) | 🇯🇵 [日本語](#japanese) | 🇨🇳 [简体中文](#chinese) | 🇪🇸 [Español](#spanish) |
| :---: | :---: | :---: | :---: | :---: |
| 🇫🇷 [Français](#french) | 🇩🇪 [Deutsch](#german) | 🇷🇺 [Русский](#russian) | 🇸🇦 [العربية](#arabic) | 🇮🇳 [हिन्दी](#hindi) |

---

<a id="english"></a>
## ⚡ Executive Overview

I am **Hyojun Jo** — a systems software engineer and infrastructure architect dedicated to high-performance runtimes, OS-native telemetry, and autonomous AI developer tooling.

My focus centers on the intersection of **low-level systems and AI-native workflows**:
- Eliminating driver overhead through user-mode Windows Filtering Platform (WFP) and Linux eBPF primitives.
- Designing strict, token-efficient Model Context Protocol (MCP) servers that prevent LLM context bleed and hallucinations.
- Enforcing orthodox engineering standards: deterministic state machines, standard-library-first design, and zero-leak memory lifecycles.

---

<a id="korean"></a>
## 🏛️ 엔지니어링 철학 및 핵심 원칙 (Core Principles)

```yaml
engineer:
  name: Hyojun Jo (조효준)
  role: Systems Architect & AI Tooling Engineer
  location: Seoul, Republic of Korea
  values:
    - "Orthodox Engineering: Standard libraries before bloated dependencies"
    - "Zero Driver: Pure user-mode WFP & eBPF over invasive kernel drivers"
    - "Token Efficiency: Compressed, normalized schemas (<1,500 tokens) for LLMs"
    - "Deterministic Lifecycles: Zero-zombie processes and leak-free memory"
```

1. **정통파 엔지니어링 (Orthodox Engineering)**:
   - 과도한 서드파티 패키지 의존성을 지양하고, 시스템 기본 API와 제1원리(First-Principles)에 기반하여 유지보수성과 견고성을 보장합니다.
2. **비침습적 텔레메트리 (Zero-Driver Telemetry)**:
   - Npcap 등 무거운 커널 드라이버 없이 네이티브 OS 필터링 엔진을 직접 제어하여 시스템 안정성을 유지합니다.
3. **결정론적 AI 에이전트 연동 (Deterministic Agent Runtimes)**:
   - AI 에이전트가 소프트웨어 빌드 및 디버깅을 수행할 때 정확한 행동을 유도할 수 있도록 엄격한 타입 검증과 즉각적인 종료 코드 피드백을 제공합니다.

---

## 🛠️ Comprehensive Technology Stack

| 계층 (Domain) | 핵심 기술 및 프레임워크 (Core Stack) |
| :--- | :--- |
| **Languages & Runtimes** | `Rust`, `Go`, `C/C++`, `TypeScript`, `Node.js (v20+)`, `Python`, `PowerShell Core` |
| **Network & Telemetry** | `Windows Filtering Platform (WFP)`, `Linux eBPF`, `Raw Sockets`, `Zero-Copy RingBuffer` |
| **AI Protocols & Tooling** | `Model Context Protocol (MCP v1.0)`, `Chrome DevTools Protocol (CDP)`, `JSON-RPC 2.0` |
| **Security & Cryptography** | `Windows DPAPI`, `X25519 (age)`, `Ed25519 (minisign)`, `AST-Level Defensive Patching` |
| **Infrastructure & CI/CD** | `GitHub Actions`, `GitLab CI`, `Containerless Micro-daemons`, `Multi-Platform Sync` |

---

## 📂 Key Architecture & Open-Source Projects

### 🌐 `netvibe` — Zero-Driver Process Network MCP
- **Overview**: Pure Rust 기반의 독립형 고성능 네트워크 리버스 엔지니어링 및 트래픽 셰이핑 MCP 서버.
- **Key Features**:
  - Wireshark/Npcap 설치 없이 특정 PID 프로세스 소켓 트래픽만 99.9% 노이즈 없이 정밀 격리 캡처.
  - LLM 컨텍스트 한계 극복을 위한 고밀도 토큰 압축 스키마(<1,500 토큰).
  - 1-Click OpenAPI 3.1 명세 및 클라이언트 SDK(Python/TS/Go) 역합성 지원.

### 🛡️ `Autonomous MCP Agent Harness`
- **Overview**: AI 에이전트의 로컬 및 클라우드 협업을 위한 무인 자율 개발 런타임.
- **Key Features**:
  - 비대화형 세션 격리(Session 0)를 탈출하는 GUI 프로세스 위임 아키텍처.
  - 백그라운드 무한 대기를 원천 차단하는 Zero-Zombie 프로세스 라이프사이클 가드.

---

<a id="japanese"></a>
### 🇯🇵 日本語概要
システムの堅牢性と決定論的なAIエージェント開発環境を追求するシステムアー키テクトです。Rust、Go、WFP/eBPF技術を活用し、不要な依存関係のない高性能な開発者向けインフラとModel Context Protocol (MCP)サーバーを構築しています。

<a id="chinese"></a>
### 🇨🇳 中文概述
致力于构建高可靠性、确定性的AI原生开发者基础设施的系统架构师。专注使用 Rust、Go 与原生操作系统原语（WFP、eBPF），打造无需驱动的高性能网络遥测与 Model Context Protocol (MCP) 工具体系。

<a id="spanish"></a>
### 🇪🇸 Resumen en Español
Arquitecto de sistemas enfocado en herramientas de desarrollo de alto rendimiento y telemetría de red sin controladores. Diseño servidores MCP rigurosos y entornos deterministas para agentes de IA con Rust y Go.

<a id="french"></a>
### 🇫🇷 Résumé en Français
Architecte de systèmes dédié aux infrastructures de développement déterministes et à la télémétrie réseau sans pilote. Conception de serveurs Model Context Protocol (MCP) optimisés en Rust et Go.

<a id="german"></a>
### 🇩🇪 Deutsche Zusammenfassung
Systemarchitekt für deterministische Entwicklertools und treiberlose Netzwerktelemetrie. Entwicklung hochperformanter Model Context Protocol (MCP) Server und robuster Agent-Runtimes mit Rust und Go.

<a id="russian"></a>
### 🇷🇺 Кратко на русском
Системный архитектор и инженер по инструментам для ИИ-агентов. Разработка высокопроизводительных серверов Model Context Protocol (MCP) и безинтерфейсной сетевой телеметрии на Rust и Go.

<a id="arabic"></a>
### 🇸🇦 نبذة بالعربية
مهندس معماري لأنظمة البرمجيات وأدوات الذكاء الاصطناعي عالية الأداء. متخصص في القياس عن بُعد للشبكات بدون برامج تشغيل وخوادم بروتوكول سياق النموذج (MCP) باستخدام Rust وGo.

<a id="hindi"></a>
### 🇮🇳 हिन्दी सारांश
उच्च-प्रदर्शन सिस्टम सॉफ्टवेयर और एआई एजेंट इन्फ्रास्ट्रक्चर में विशेषज्ञता प्राप्त सिस्टम आर्किटेक्ट। Rust और Go का उपयोग करके बिना ड्राइवर के नेटवर्क टेलीमेट्री और मॉडल संदर्भ प्रोटोकॉल (MCP) का निर्माण।

---

## 📬 Connectivity & Platforms

- **GitHub**: [github.com/jo060235354-design](https://github.com/jo060235354-design)
- **GitLab**: [gitlab.com/jo060235354](https://gitlab.com/jo060235354)
- **Hugging Face**: [huggingface.co/sfmiko](https://huggingface.co/sfmiko)
- **Direct Mail**: `jo060235354@gmail.com`
