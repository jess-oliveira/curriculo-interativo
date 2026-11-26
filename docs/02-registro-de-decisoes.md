# 📝 Registro de Decisões do Projeto

## 1. Navegação e estrutura da página

- O currículo será desenvolvido em uma única página, em vez de várias páginas.
- O menu de navegação terá links para as seções da própria página.
- As seções previstas são:
  - Sobre mim;
  - Habilidades;
  - Formação;
  - Experiência profissional;
  - Contato.
- Inicialmente, todo o conteúdo do currículo estará visível, sem necessidade de aplicar filtros.

## 2. Organização e filtros de habilidades

- As habilidades serão organizadas em categorias ou tópicos, de acordo com suas áreas de conhecimento.
- Entre os tópicos inicialmente previstos estão:
  - Testes de software;
  - Ferramentas;
  - Linguagens de programação;
  - Banco de dados;
  - Metodologias;
  - Competências comportamentais.
- Cada tópico terá um menu expansível com as habilidades disponíveis para seleção.
- O recrutador poderá selecionar uma ou várias habilidades dentro de um mesmo tópico ou de tópicos diferentes.
- Os resultados serão atualizados imediatamente a cada seleção, sem necessidade de um botão para aplicar os filtros.
- Após a seleção, somente as habilidades selecionadas serão exibidas na área de resultados.
- Os tópicos de filtros permanecerão disponíveis para permitir novas seleções, mesmo quando outras habilidades estiverem ocultas.
- Haverá um botão **Limpar filtros**, que restaurará a visualização completa das habilidades.
- Será apresentada uma orientação ao recrutador: “Para visualizar detalhes e evidências das habilidades, selecione uma ou mais habilidades de interesse.”

## 3. Exibição das evidências práticas

- As demonstrações práticas serão exibidas dentro da própria página, sem utilização de janelas modais.
- A demonstração será apresentada por meio de um disclosure expansível.
- Ao expandir o disclosure, o conteúdo será exibido na página, empurrando os elementos seguintes para baixo.
- Ao recolher o disclosure, somente a demonstração prática será ocultada.
- Uma habilidade poderá ter várias evidências práticas.
- Uma mesma evidência poderá estar relacionada a várias habilidades.
- As demonstrações práticas serão apresentadas quando houver um projeto ou material que permita comprovar a aplicação da habilidade.
- Quando não houver evidência prática disponível, não será apresentada uma opção de demonstração vazia.

## 4. Exibição das informações relacionadas às habilidades

Cada habilidade apresentada terá os seguintes elementos, quando aplicáveis:

1. **Título da habilidade:** elemento principal, com maior destaque visual.
2. **Disclosure:** demonstração prática da habilidade, com um trecho relevante do projeto e link para acessar o repositório completo no GitHub, quando houver evidência disponível.
3. **Formação relacionada:** bloco visualmente secundário, apresentado abaixo do disclosure e sempre visível quando houver formação ou curso associado à habilidade.

Outras decisões:

- Uma mesma habilidade poderá estar relacionada a várias formações e cursos.
- Uma mesma habilidade poderá ter sido desenvolvida em mais de uma formação ou curso.
- As informações de formação não serão ocultadas ao expandir ou recolher o disclosure.
- A demonstração prática será específica para a habilidade apresentada, mesmo quando o projeto utilizado como evidência estiver relacionado a outras habilidades.
- A ausência de uma demonstração prática não impedirá a apresentação da habilidade e de sua formação relacionada.

## 5. Usuários e permissões

- O público principal será formado por recrutadores interessados em consultar o currículo.
- Não haverá login ou autenticação na primeira versão.
- Não haverá painel administrativo na primeira versão.
- As informações serão atualizadas diretamente nos arquivos do projeto.
- Uma possível área administrativa poderá ser considerada em uma versão futura.

## 6. Tecnologias e qualidade

### 6.1. Tecnologias previstas

- HTML, CSS e JavaScript para o front-end.
- Git e GitHub para versionamento e hospedagem do repositório.
- Cypress para automação de testes.

### 6.2. Práticas de qualidade previstas

- Testes manuais.
- Testes funcionais.
- Testes exploratórios.
- Verificação de responsividade.
- Verificação da navegação.
- Verificação de acessibilidade.