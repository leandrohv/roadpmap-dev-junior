# Roadmap Zero → Júnior (26 semanas)

Programa completo para levar alunos do **zero** a **programador(a) júnior sólido(a)**, com foco em **fundamentos**, **projetos práticos**, **segurança por padrão** e **portfólio público**.

> **Como usar:** faça fork/clone deste repositório, siga o cronograma por fases, registre seus projetos em subpastas e abra Pull Requests semanais (auto‑review).

---

## 🧭 Sumário
- [🎯 Objetivos de aprendizagem](#objetivos-de-aprendizagem)
- [🧰 Pré-requisitos e ambiente](#pre-requisitos-e-ambiente)
  - [Convenções do repositório](#convencoes-do-repositorio)
- [🧱 Pilares e trilhas de estudo](#pilares-e-trilhas-de-estudo)
  - [1) Algoritmos com Portugol](#1-algoritmos-com-portugol)
  - [2) Banco de Dados SQL](#2-banco-de-dados-sql)
  - [3) Linguagens & Frameworks](#3-linguagens-frameworks)
- [🗓️ Cronograma por fases (26 semanas)](#cronograma-por-fases-26-semanas)
- [🛡️ Segurança por padrão](#seguranca-por-padrao)
  - [Referenciais essenciais](#referenciais-essenciais)
  - [Práticas mínimas](#praticas-minimas)
  - [Tooling por projeto](#tooling-por-projeto)
- [✅ Checklists de segurança](#checklists-de-seguranca)
  - [Aplicação](#aplicacao)
  - [Pipeline/Repo](#pipeline-repo)
- [📺 Canais e playlists recomendados (PT-BR + EN)](#canais-e-playlists-recomendados-pt-br-en)
- [🧪 Rubrica de proficiência (Selo Júnior)](#rubrica-de-proficiencia-selo-junior)
- [📦 Entregáveis por fase](#entregaveis-por-fase)
- [📄 Licença](#licenca)

<a id="objetivos-de-aprendizagem"></a>
## 🎯 Objetivos de aprendizagem
- Raciocínio lógico e **algoritmos** com **Portugol** (pseudocódigo).
- **Banco de dados SQL** (modelagem, DDL/DML, JOINS, transações).
- Uma **linguagem principal** (PHP _ou_ Java _ou_ Python) e uma **web framework** popular.
- **Git/GitHub** (branching, PRs, issues, releases, actions básicas).
- **Testes**, **logs**, **lint/format**, **CI** e **containers** básicos.
- **Segurança by design**: OWASP Top 10/API, **auth** (JWT/OAuth2), **secret scanning**, **SAST/DAST**, **SBOM**, **CodeQL/Dependabot**, **LGPD básica**.
- Projetos públicos com documentação (README, coleções de API, Dockerfile).

**Selo Júnior (meta):** ✔✔ em todos os pilares e ✔✔✔ em 2–3 deles (ver rubrica).

---

<a id="pre-requisitos-e-ambiente"></a>
## 🧰 Pré-requisitos e ambiente
- **VS Code** + extensões da linguagem escolhida
- **Git** + conta no **GitHub** (chave SSH)
- **Docker** (opcional, recomendado para DBs/serviços)
- **MySQL/PostgreSQL**, **DBeaver** (GUI) e **Postman/Insomnia** (APIs)

<a id="convencoes-do-repositorio"></a>
### Convenções do repositório
```text
/roadmap
  /fase-01/...
  /fase-02/...
  /projetos/
    /00-portugol/
    /01-sql/
    /02-web-linguagem/
    /03-api-segura/
  README.md  ← este arquivo
```

---

<a id="pilares-e-trilhas-de-estudo"></a>
## 🧱 Pilares e trilhas de estudo

<a id="1-algoritmos-com-portugol"></a>
### 1) Algoritmos com **Portugol**
- Variáveis, E/S, condicionais, loops, vetores/matrizes, funções e recursão.
- Complexidade (noções), decomposição, testes de mesa.  
**Projeto:** 20–30 exercícios + mini‑sistema de terminal.

<a id="2-banco-de-dados-sql"></a>
### 2) Banco de Dados **SQL**
- Modelagem (DER), chaves, normalização; DDL/DML; **JOINs**, `GROUP BY`, `HAVING`, índices; transações/isolamento.  
**Projeto:** esquema para app (usuários/produtos/pedidos), seeds e 10 consultas.

<a id="3-linguagens-frameworks"></a>
### 3) Linguagens & Frameworks
**a) PHP (Laravel)** – Rotas, controllers, Eloquent, validação, migrations/seeders, auth (Sanctum/Passport); CSRF, policies/gates.  
**b) Java (Spring Boot)** – REST, JPA, Bean Validation, profiles; **Spring Security** (JWT/OAuth2), CORS, roles, actuator protegido.  
**c) Python (Django/FastAPI)** – Django: ORM, DRF, SecurityMiddleware; FastAPI: Pydantic, dependências, OAuth2 + JWT, CORS.

---

<a id="cronograma-por-fases-26-semanas"></a>
## 🗓️ Cronograma por fases (26 semanas)
> **Cadência sugerida:** 10–12h/semana. Ajuste conforme sua realidade.

**Fase 1 (Semanas 1–4) — Fundamentos & Portugol**  
Lógica, tipos, estruturas de controle, funções, vetores/matrizes; 1 mini‑projeto em Portugol (menu/relatórios).

> **Vídeos e Treinamentos - Portugol & Algoritmos**
- Portugol Webstudio (online): https://portugol.dev/  
- Portugol Studio (desktop): https://github.com/UNIVALI-LITE/Portugol-Studio  
- **Algoritmos – Curso em Vídeo (playlist):** https://www.youtube.com/playlist?list=PLHz_AreHm4dkZ9-atkcmcBaMZdmLHft8n  
- **Algoritmos I – UNIVESP (playlist):** https://www.youtube.com/playlist?list=PLxI8Can9yAHcUdIGv9aaZqkt-z0fepFa8  

---

**Fase 2 (Semanas 5–6) — Git/GitHub & Sistema**  
Branches, PR, merge/rebase, tags, releases, Actions simples. Ambiente com Docker e `.env` (sem segredos no Git).

> **Vídeos e Treinamentos — Git & GitHub**
- **Git/GitHub para Iniciantes – Rafaella Ballerini (playlist):** https://www.youtube.com/playlist?list=PLlAbYrWSYTiPA2iEiQ2PF_A9j__C4hi0A  
- **Git/GitHub na Vida Real – Willian Justen (playlist):** https://www.youtube.com/playlist?list=PLlAbYrWSYTiNqugqFFWWsgONJsmc3eMpg  

---

**Fase 3 (Semanas 7–10) — SQL & Modelagem**  
DER, normalização, DDL/DML, **JOINs**, agregações, índices, transações; projeto SQL com carga e consultas.

> **Vídeos e Treinamentos — SQL**
- **MySQL – Curso em Vídeo (playlist):** https://www.youtube.com/playlist?list=PLHz_AreHm4dkBs-795Dsgvau_ekxg8g1r  
- **SQL (T‑SQL/SQL Server) – Bóson Treinamentos (playlist):** https://www.youtube.com/playlist?list=PLucm8g_ezqNqI5cW3alteV5olcMCcHYRK  
- **SQL Injection (vídeo PortSwigger):** https://www.youtube.com/watch?v=wX6tszfgYp4  

---

**Fase 4 (Semanas 11–16) — Web/API na linguagem escolhida**  
**PHP (Laravel)** _ou_ **Java (Spring Boot)** _ou_ **Python (Django/FastAPI)**. CRUD, validação, **auth** (JWT/OAuth2), camadas, testes, logs, OpenAPI.

> **Vídeos e Treinamentos — Web/API por linguagem**
**PHP (Laravel)**  
- **PHP Moderno – Curso em Vídeo (playlist):** https://www.youtube.com/playlist?list=PLHz_AreHm4dlFPrCXCmd5g92860x_Pbr_  
- **Laravel 12 – Celke (playlist):** https://www.youtube.com/playlist?list=PLmY5AEiqDWwB29FbhTfTh86Zr0yjeFBwO  
- **Segurança no PHP (playlist EN – visão geral):** https://www.youtube.com/playlist?list=PL2407F4EE0530B251  

**Java (Spring Boot/Security)**  
- **Maratona Java – DevDojo (playlist):** https://www.youtube.com/playlist?list=PL62G310vn6nFIsOCC0H-C2infYgwm8SWW  
- **Spring Boot – Michelli Brito (playlist):** https://www.youtube.com/playlist?list=PL8iIphQOyG-DHLpEx1TPItqJamy08fs1D  
- **Spring Security + JWT (vídeo):** https://www.youtube.com/watch?v=t6prPki7daU  

**Python (Django/FastAPI)**  
- **Python – Curso em Vídeo (playlist):** https://www.youtube.com/playlist?list=PLHz_AreHm4dlKP6QQCekuIPky1CiwmdI6  
- **Django Security (talk):** https://www.youtube.com/watch?v=33Bb8QTfQ-M  
- **FastAPI OAuth2 + JWT (docs):** https://fastapi.tiangolo.com/tutorial/security/oauth2-jwt/  
- **FastAPI Authentication (vídeo):** https://www.youtube.com/watch?v=oEhyMoHkPTE  


---

**Fase 5 (Semanas 17–22) — Segurança aplicada + CI**  
OWASP Top 10 / API Top 10, headers, rate limit, RBAC, migrações; SAST/DAST, SBOM, CodeQL/Dependabot; checagens em PR.


> **Vídeos e Treinamentos — Segurança aplicada + CI**
- **OWASP Top 10 (playlist oficial):** https://www.youtube.com/@OWASPGLOBAL/search?query=owasp%20top%2010  
- **OWASP API Security Top 10 (vídeos):** https://www.youtube.com/results?search_query=owasp+api+security+top+10  
- **OWASP ZAP (playlist oficial):** https://www.youtube.com/playlist?list=PLEBitBW-Hlsv8cEIUntAO8st2UGhmrjUB  
- **Semgrep (playlist):** https://www.youtube.com/@semgrep/playlists  
- **Bandit (vídeo):** https://www.youtube.com/watch?v=dGkmAolcpxE  
- **CodeQL (vídeo introdutório):** https://www.youtube.com/watch?v=y_-pIbsr7jc  
- **Trivy/SBOM CycloneDX (vídeo):** https://www.youtube.com/watch?v=YlDVnaKuffo  


---

**Fase 6 (Semanas 23–26) — Portfólio & Entrevista**  
Refino do projeto final, deploy simples (Docker Compose/serviço grátis), README impecável, issues/roadmap, vídeo demo curto.

> **Vídeos e Treinamentos — Portfólio & Entrevista**
- **OWASP (canal):** https://www.youtube.com/c/OWASPGLOBAL/playlists  
- **ZAP (canal):** https://www.youtube.com/playlist?list=PLH8n_ayg-60J9i3nsLybper-DR3zJw6Z5  
- **PortSwigger (W. Security Academy):** https://www.youtube.com/playlist?list=PLoX0sUafNGbFcyjCwB0N7x_Zxw7T1-I9Y  

---

<a id="seguranca-por-padrao"></a>
## 🛡️ Segurança por padrão

<a id="referenciais-essenciais"></a>
### Referenciais essenciais
- **OWASP Top 10 (Web)**: https://owasp.org/www-project-top-ten/  
- **OWASP API Security Top 10 (2023)**: https://owasp.org/API-Security/  
- **OWASP ASVS**: https://owasp.org/www-project-application-security-verification-standard/  
- **NIST SSDF (SP 800‑218)**: https://csrc.nist.gov/Projects/ssdf  
- **SLSA (Supply chain)**: https://slsa.dev/  
- **LGPD (Brasil)**: https://www.gov.br/cidadania/pt-br/acesso-a-informacao/lgpd

<a id="praticas-minimas"></a>
### Práticas mínimas
- Input validation; **prepared statements/ORM**; senha com **bcrypt/argon2**; **RBAC**; logs sem PII sensível; **headers** (HSTS/CSP/NoSniff); **rate limit**; **CORS** estrito.
- **Laravel**: `@csrf`, `FormRequest`/validação, `Gate/Policy`, Sanctum/Passport, `APP_KEY` secreto (em `.env`).  
- **Spring**: `spring-boot-starter-security`, JWT/OAuth2, `@Validated`, CORS explícito, actuator protegido.  
- **Django**: `SecurityMiddleware`, `SECURE_*`, `CSRF_COOKIE_SECURE`, `SESSION_COOKIE_SECURE`, `PASSWORD_HASHERS`.  
- **FastAPI**: OAuth2 Password + JWT, `passlib[bcrypt]`, `Depends` p/ autorização, middlewares (CORS/rate limit).

<a id="tooling-por-projeto"></a>
### Tooling por projeto
- **Secret scanning**: **Gitleaks** – https://github.com/gitleaks/gitleaks  
- **SAST**: **Semgrep** – https://semgrep.dev/ • **Bandit** (Python) – https://bandit.readthedocs.io/  
- **Dependências**: **pip‑audit** – https://github.com/pypa/pip-audit • `npm audit` • `composer audit` • OWASP Dependency-Check  
- **DAST**: **OWASP ZAP** – https://www.zaproxy.org/  
- **SBOM**: **CycloneDX** – https://cyclonedx.org/ (pode gerar via **Trivy**)  
- **GitHub**: **Dependabot** • **CodeQL** (code scanning).

---

<a id="checklists-de-seguranca"></a>
## ✅ Checklists de segurança

<a id="aplicacao"></a>
### Aplicação
- [ ] Senhas com bcrypt/argon2; tokens com expiração/refresh.  
- [ ] SQL apenas **parametrizado** (ORM/Query Builder).  
- [ ] **Headers**: HSTS, CSP, X‑Frame‑Options, X‑Content‑Type‑Options; CORS estrito.  
- [ ] **Validação** server‑side; mensagens de erro genéricas.  
- [ ] **Logs** sem dados sensíveis; correlação de requisições.  
- [ ] **Rate limit** e limites de payload.  
- [ ] **Backups** e restauração testada (DB).

<a id="pipeline-repo"></a>
### Pipeline/Repo
- [ ] `.env` e segredos **fora do Git**; secrets em vault/Actions.  
- [ ] **Gitleaks** em _pre‑commit_ + CI; rotação de segredos se vazarem.  
- [ ] **Semgrep/Bandit** no PR; _quality gate_.  
- [ ] **Dependabot** e auditorias; CVEs críticas quebram o build.  
- [ ] **CodeQL** ativo; **SBOM CycloneDX** anexada à release.  
- [ ] **ZAP Baseline** em PR da API.

---

<a id="canais-e-playlists-recomendados-pt-br-en"></a>
## 📺 Canais e playlists recomendados (PT-BR + EN)
- **OWASP (oficial):** https://www.youtube.com/c/OWASPGLOBAL/playlists  
- **Michelli Brito (Spring/Java):** https://www.youtube.com/michellibrito  
- **DevDojo (Java):** https://www.youtube.com/@DevDojoBrasil/playlists  
- **Amigoscode (Spring/Java):** https://www.youtube.com/c/amigoscode/playlists  
- **Curso em Vídeo (Gustavo Guanabara):** https://www.youtube.com/c/CursoemV%C3%ADdeo/playlists  
- **Bóson Treinamentos:** https://www.youtube.com/@bosontreinamentos/playlists  

---

<a id="rubrica-de-proficiencia-selo-junior"></a>
## 🧪 Rubrica de proficiência (Selo Júnior)
**Fundamentos** – Portugol (20+ exercícios) e SQL intermediário.  
**Web/API** – CRUD REST + validação + testes + documentação; autenticação (JWT/OAuth2) com roles.  
**Segurança** – Secret scanning, SAST/DAST, SBOM, CodeQL, headers ativos e SQL parametrizado.  
**Engenharia** – GitFlow simples, PRs revisados, releases versionadas, logs estruturados e README impecável.

---

<a id="entregaveis-por-fase"></a>
## 📦 Entregáveis por fase
1. **F1:** exercícios Portugol + mini‑projeto.  
2. **F2:** repositório Git organizado + workflow CI mínimo.  
3. **F3:** schema SQL, seeds e 10 queries úteis.  
4. **F4:** API REST (linguagem escolhida) com autenticação e testes.  
5. **F5:** Pipeline com Gitleaks, Semgrep/Bandit, ZAP Baseline, SBOM, CodeQL.  
6. **F6:** Projeto final polido, demo (2–5 min), README e roadmap.

---

<a id="licenca"></a>
## 📄 Licença
MIT License – use/adapte com créditos.  
Última atualização: **29/08/2025**.  
Elaborado por: **Leandro Venâncio**  
Me segue nas redes sociais: https://linktr.ee/leandro.venancio
