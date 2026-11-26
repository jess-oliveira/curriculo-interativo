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

O projeto também tem como objetivo aplicar conhecimentos de análise de requisitos, modelagem de sistemas, desenvolvimento web, versionamento e testes de software.

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

- O recrutador acessa a página profissional.
- Visualiza as informações organizadas em seções.
- Consulta habilidades técnicas e competências comportamentais.
- Utiliza filtros por categorias e habilidades de interesse.
- Visualiza somente as habilidades selecionadas após a aplicação dos filtros.
- Consulta demonstrações práticas associadas às habilidades, quando houver evidências disponíveis.
- Permite adicionar ou remover habilidades da seleção, atualizando automaticamente os resultados exibidos.
- Consulta formações e cursos relacionados às habilidades.
- Acessa LinkedIn, GitHub e informações de contato.

# 5. Escopo do projeto

### 5.1. Dentro do escopo (In Scope)

- Apresentação profissional.
- Experiências profissionais.
- Formação acadêmica e cursos.
- Habilidades técnicas (Hard Skills).
- Competências comportamentais (Soft Skills).
- Filtros por categorias e habilidades.
- Seleção de uma ou várias habilidades.
- Exibição dos resultados conforme os filtros selecionados.
- Limpeza dos filtros.
- Exibição de evidências práticas associadas às habilidades, quando disponíveis.
- Exibição de formações e cursos relacionados às habilidades.
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

6.1. Requisitos funcionais (RF)
| ID | Requisito |
| -- | --------- |
RF01|  Exibir informações pessoais e profissionais.
RF02|	Exibir experiências profissionais.
RF03|	Exibir formação acadêmica e cursos.
RF04|	Exibir habilidades técnicas (Hard Skills).
RF05|	Exibir competências comportamentais (Soft Skills).
RF06|	Organizar as habilidades por categorias.
RF07|	Disponibilizar as habilidades para seleção nos filtros.
RF08|	Permitir a seleção múltipla de habilidades, inclusive de categorias diferentes.
RF09|	Atualizar os resultados automaticamente após a seleção dos filtros.
RF10|	Exibir somente as habilidades correspondentes aos filtros selecionados.
RF11|	Manter as categorias de filtros disponíveis durante a filtragem.
RF12|	Permitir limpar os filtros e restaurar a visualização completa.
RF13|	Exibir demonstrações práticas expansíveis, com links para os projetos completos no GitHub, quando houver evidências disponíveis.
RF14|	Exibir formações e cursos relacionados às habilidades.
RF15|	Manter as informações de formação visíveis independentemente da demonstração prática estar expandida ou recolhida.
RF16|	Disponibilizar um menu de navegação entre as seções da página.
RF17|	Disponibilizar acesso ao perfil profissional no LinkedIn.
RF18|	Disponibilizar acesso ao perfil no GitHub.
RF19|	Disponibilizar contato pelo WhatsApp.

## 6.2. Requisitos não funcionais (RNF)

| ID | Requisito |
| --- | --- |
RNF01|	A aplicação deve possuir layout responsivo.
RNF02|	Deve funcionar nos principais navegadores modernos.
RNF03|	Deve apresentar boa legibilidade e organização visual.
RNF04|	Deve possuir navegação intuitiva.
RNF05|	A aplicação deverá apresentar desempenho adequado durante o carregamento e a utilização dos filtros.
RNF06|	Deve permitir navegação por teclado e considerar critérios de acessibilidade.
RNF07|	O código deve possuir organização, legibilidade e separação de responsabilidades, facilitando sua manutenção.
RNF08|	A documentação técnica do projeto deve ser clara e organizada, facilitando a compreensão e a manutenção.

# 7. Regras de negócio (RN)

| ID | Regra |
|---|----------|
RN01| O recrutador terá acesso somente para consulta das informações.
RN02|	A atualização das informações será realizada diretamente nos arquivos do projeto.
RN03|	As habilidades deverão ser organizadas conforme suas categorias de conhecimento.
RN04|	Uma habilidade poderá estar relacionada a mais de uma formação ou curso.
RN05|	Uma habilidade poderá possuir mais de uma evidência prática associada.
RN06|	Uma mesma evidência prática poderá estar relacionada a diferentes habilidades.
RN07|	Somente habilidades correspondentes aos filtros selecionados deverão ser exibidas.
RN08|	Ao limpar os filtros, todas as habilidades deverão voltar a ser exibidas.
RN09|	A demonstração prática somente será disponibilizada quando houver evidência relacionada à habilidade.
RN10|	As informações de formação deverão permanecer visíveis independentemente de a demonstração prática estar expandida ou recolhida.
RN11|	A ausência de evidência prática não impedirá a apresentação da habilidade e de sua formação relacionada, quando houver.

# 8. Restrições e limitações

| ID | Restrição ou limitação |
|-|-|
RL01|	A primeira versão não possuirá painel administrativo.
RL02|	A aplicação não possuirá sistema de login ou autenticação.
RL03|	As informações serão atualizadas diretamente nos arquivos do projeto.
RL04|	Não haverá banco de dados para armazenamento dinâmico das informações.
RL05|	A manutenção do currículo dependerá de alterações manuais no conteúdo da aplicação.

**Documento elaborado durante a fase de concepção e análise de requisitos.**
