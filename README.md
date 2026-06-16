# ilha_sql
# 🏝 Ilha SQL

Jogo educacional web para ensinar SQL na prática a adolescentes. O aluno cria um personagem, cai numa ilha misteriosa após um acidente aéreo e precisa usar comandos SQL reais para descobrir quem está na ilha e encontrar um piloto que o ajude a escapar.

![Ilha SQL](https://img.shields.io/badge/SQL-Educacional-f5c842?style=for-the-badge&logo=sqlite&logoColor=black)
![Status](https://img.shields.io/badge/Status-Em%20desenvolvimento-2ecc71?style=for-the-badge)
![Stack](https://img.shields.io/badge/Stack-HTML%20%2B%20JS%20puro-4fc3f7?style=for-the-badge)

---

## 🎮 Como funciona

O aluno escolhe uma turma (via PIN criado pelo professor), cria um personagem com nome e avatar pixel art e entra na ilha. O objetivo narrativo é descobrir quem está no lugar e encontrar um piloto para escapar — tudo usando SQL real.

O jogo tem **10 regiões** num mapa estilo Mario, desbloqueadas em sequência. Cada região é uma fase com 5–6 missões que ensinam um conceito SQL progressivo:

| Região | Conceito |
|--------|----------|
| 🌳 Floresta SELECT | `SELECT`, `INSERT` |
| 🏖 Praia dos Filtros | `WHERE` |
| 🕳 Caverna das Decisões | `AND`, `OR` |
| 🍃 Bosque dos Padrões | `LIKE` |
| 🌊 Lago da Organização | `ORDER BY` |
| 🏘 Vila dos Registros | `UPDATE` |
| ⚓ Porto das Limpezas | `DELETE` |
| 🏛 Templo dos Cálculos | `COUNT`, `SUM`, `AVG` |
| 🏰 Fortaleza dos Clãs | `GROUP BY` |
| 👑 Castelo das Conexões | `JOIN` |
| ✈ Pista de Resgate | Desafio final |

Em cada missão, a **Natty** (guia fantasma da ilha) apresenta um contexto narrativo e o aluno digita um comando SQL real num terminal integrado. O sistema valida a query automaticamente, dá feedback e libera a próxima missão ao acertar.

O banco de dados da ilha tem personagens famosos (Neymar, Anitta, Batman, Beyoncé e outros), tornando as consultas divertidas e contextualizadas.

---

## 👨‍🏫 Painel do professor

- Cria turmas com PIN de 4 dígitos
- Alunos entram digitando o PIN (sem precisar selecionar a turma manualmente)
- Visualiza ranking por XP de cada turma
- Identifica alunos travados (sem progresso)

---

## 🚀 Como usar

### Opção 1 — GitHub Pages (recomendado)
1. Faça um fork deste repositório
2. Vá em **Settings → Pages**
3. Selecione a branch `main` e a pasta `/ (root)`
4. Acesse a URL gerada — pronto

### Opção 2 — Local
Baixe o arquivo `ilha_sql.html` e abra no navegador. Não precisa de servidor.

---

## 🛠 Stack

- **HTML + CSS + JS puro** — sem frameworks, sem build
- **[sql.js](https://github.com/sql-js/sql.js/)** — SQLite compilado para WebAssembly, roda no browser
- **localStorage** — salva progresso por turma, nome e senha, sem servidor
- **Pixel art** gerado em Canvas 2D

---

## 💾 Persistência de dados

O progresso dos alunos é salvo no **localStorage do navegador**. Isso significa:

- ✅ Funciona offline e sem backend
- ✅ Ideal para laboratórios de informática com máquinas fixas
- ⚠️ O progresso fica vinculado ao navegador da máquina usada
- ⚠️ Trocar de computador reinicia o progresso

> Integração com banco de dados em nuvem (Supabase) planejada para versões futuras.

---

## 📚 Inspiração

Inspirado no [SQL Island](https://sql-island.informatik.uni-kl.de/) de Johannes Schildgen (Technische Universität Kaiserslautern, Alemanha), adaptado para o contexto brasileiro com narrativa própria, personagens locais e sistema de turmas para uso em sala de aula.

---

## 📄 Licença

Projeto educacional desenvolvido para o SENAI/SESI. Uso livre para fins educacionais.
