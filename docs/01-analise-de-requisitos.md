# Documento de Análise de Requisitos
## Projeto: Currículo Interativo

**Versão:** 0.1 — Levantamento inicial  
**Status:** Em elaboração  
**Responsável pelo projeto:** Jéssica Oliveira  
**Tipo de projeto:** Aplicação Web

---

# 1. Identificação e objetivo do projeto

Desenvolver um currículo profissional interativo, que também funcione como demonstração prática dos conhecimentos em Análise e Modelagem de Sistemas, Desenvolvimento e Quality Assurance (QA).

O projeto busca substituir a apresentação profissional estática em PDF por uma aplicação web que permita ao recrutador consultar informações profissionais, filtrar competências e acessar evidências práticas dos conhecimentos apresentados.

# 2. Público-alvo e envolvidos

### 2.1. Proprietária do currículo
Responsável pelas informações apresentadas e pela atualização dos dados profissionais e acadêmicos.

### 2.2. Recrutadores
Público que acessará a aplicação para consultar o perfil profissional, experiências, formação, competências e projetos.

**Observação:** Na primeira versão, não haverá painel administrativo nem necessidade de autenticação. A atualização das informações será realizada diretamente nos arquivos do projeto.

# 3. Contexto e necessidade

Atualmente, as informações profissionais são apresentadas por meio de um currículo em PDF.

Embora o documento reúna as informações necessárias, sua estrutura é estática e exige que o recrutador localize manualmente as competências e experiências que procura.

Além disso, a inclusão de novas informações pode exigir ajustes na organização e no layout do documento.

A proposta é desenvolver uma aplicação web que facilite a consulta das informações e permita a visualização de evidências relacionadas às competências apresentadas.

# 4. Análise do processo — AS IS e TO BE

### 4.1. AS IS — Processo atual

**Currículo em PDF — Documento estático**

- Recrutador acessa o documento.
- Consulta manualmente as informações.
- Localiza as competências entre as demais informações.
- Acessa outros sites por meio de links, quando disponíveis.
- Atualizações podem exigir alterações manuais no conteúdo e na organização visual do documento.

### 4.2. TO BE — Processo proposto

**Currículo interativo — Aplicação web**

- Recrutador acessa a página profissional.
- Visualiza as informações organizadas em seções.
- Consulta habilidades técnicas e comportamentais.
- Filtra competências de acordo com o que procura.
- Visualiza somente as competências selecionadas.
- Expande informações complementares e evidências associadas às competências.
- Consulta projetos e suas respectivas documentações.
- Acessa LinkedIn, GitHub e contato.

# 5. Escopo do projeto

### 5.1. Dentro do escopo (In Scope)

- Apresentação profissional.
- Experiências profissionais.
- Formação acadêmica e cursos.
- Habilidades técnicas (Hard Skills).
- Competências comportamentais (Soft Skills).
- Filtros de competências.
- Exibição de evidências associadas às habilidades.
- Documentação dos projetos.
- Links externos para LinkedIn e GitHub.
- Contato pelo WhatsApp.
- Navegação por seções em uma única página.

### 5.2. Fora do escopo (Out of Scope) — Versão 1.0

- Painel administrativo.
- Sistema de login e autenticação.
- Cadastro e atualização de informações por interface administrativa.
- Banco de dados para armazenamento dinâmico do currículo.
- Catálogo pesquisável de todas as competências existentes no mercado.

**Observação:** Os itens fora do escopo poderão ser avaliados em versões futuras.

# 6. Levantamento de requisitos

## 6.1. Requisitos funcionais (RF)

| ID | Requisito |
|---|---|
| RF01 | Exibir informações pessoais e profissionais. |
| RF02 | Exibir experiências profissionais. |
| RF03 | Exibir formação acadêmica e cursos. |
| RF04 | Exibir habilidades técnicas (Hard Skills). |
| RF05 | Exibir competências comportamentais (Soft Skills). |
| RF06 | Permitir filtrar habilidades técnicas. |
| RF07 | Permitir filtrar competências comportamentais. |
| RF08 | Exibir somente as competências correspondentes aos filtros selecionados. |
| RF09 | Permitir selecionar múltiplas competências simultaneamente. |
| RF10 | Permitir limpar os filtros e restaurar a visualização completa. |
| RF11 | Exibir evidências relacionadas às competências selecionadas. |
| RF12 | Permitir expandir informações complementares de uma competência. |
| RF13 | Permitir expandir a documentação prática dos projetos associados. |
| RF14 | Permitir recolher os conteúdos expandidos sem sair da página. |
| RF15 | Disponibilizar acesso ao LinkedIn. |
| RF16 | Disponibilizar acesso ao GitHub. |
| RF17 | Disponibilizar contato pelo WhatsApp. |
| RF18 | Disponibilizar links para documentações e materiais dos projetos. |

## 6.2. Requisitos não funcionais (RNF)

| ID | Requisito |
|---|---|
| RNF01 | A aplicação deve possuir layout responsivo. |
| RNF02 | Deve funcionar nos principais navegadores modernos. |
| RNF03 | Deve apresentar boa legibilidade e organização visual. |
| RNF04 | Deve possuir navegação intuitiva. |
| RNF05 | Deve apresentar desempenho adequado no carregamento. |
| RNF06 | Deve permitir navegação por teclado e considerar critérios de acessibilidade. |
| RNF07 | O código deve possuir organização e separação de responsabilidades. |

# 7. Regras de negócio (RN)

| ID | Regra |
|---|---|
| RN01 | O recrutador terá acesso somente para consulta das informações. |
| RN02 | A atualização das informações será realizada diretamente nos arquivos do projeto. |
| RN03 | As competências devem ser classificadas entre Hard Skills e Soft Skills. |
| RN04 | Uma competência poderá possuir mais de uma evidência associada. |
| RN05 | Uma evidência poderá estar relacionada a mais de uma competência. |
| RN06 | Ao selecionar competências nos filtros, somente as competências correspondentes deverão ser apresentadas. |
| RN07 | Ao limpar os filtros, todas as competências deverão voltar a ser exibidas. |
| RN08 | A documentação complementar deverá ser apresentada na própria página, por meio de conteúdo expansível. |

# 8. Decisões iniciais de interface e navegação

- A aplicação será organizada em uma única página.
- A navegação será dividida em seções.
- As competências serão apresentadas por categorias.
- Os filtros permitirão seleção múltipla.
- Os resultados filtrados substituirão temporariamente a visualização completa das competências.
- Cada competência poderá apresentar evidências relacionadas.
- A documentação poderá ser expandida e recolhida sem redirecionamento para outra página.
- Links externos poderão direcionar o recrutador para materiais completos no GitHub.

# 9. Pendências para validação

- Definir a organização visual definitiva das seções.
- Definir os campos e informações de cada competência.
- Definir a estrutura das evidências associadas.
- Validar a lista de habilidades e suas respectivas categorias.
- Detalhar os critérios de aceitação dos requisitos.
- Definir as tecnologias e a arquitetura da aplicação.

---

**Documento elaborado durante a fase de concepção e análise de requisitos.**

**Próxima etapa:** Refinamento e validação dos requisitos antes do início da modelagem do sistema.