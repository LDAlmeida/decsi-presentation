
### 1. **Abertura e Agradecimento (1 minuto)**

"Boa tarde a todos, meu nome é Lucas Almeida e hoje apresento o meu trabalho de conclusão de curso intitulado 'Desenvolvimento de uma plataforma de artistas monlevadenses para a Casa de Cultura de João Monlevade'.  
Gostaria de começar agradecendo aos membros da banca por estarem presentes e pela disponibilidade em avaliar meu projeto."

---

### 2. **Sumário da Apresentação (1 minuto)**

"Durante esta apresentação, abordarei os seguintes pontos:

1. Introdução e contexto do projeto;
2. Desenvolvimento e funcionalidades da plataforma;
3. Resultados obtidos a partir dos testes;
4. Conclusões e trabalhos futuros."

---

### 3. **Introdução (3 a 4 minutos)**


**Problema:**  

Leia o primeiro slide.

**Contexto e Problema:**  
"A Casa de Cultura de João Monlevade, inaugurada em 1981, desempenha um papel importante na promoção da cultura local. No entanto, ela não possuía uma plataforma digital adequada para divulgar os trabalhos dos artistas locais. Em um cenário nacional, os investimentos em cultura são bastante limitados, e há uma necessidade urgente de valorizar os talentos locais, especialmente em cidades menores como João Monlevade."

**Objetivo Geral:**  
"O objetivo do meu trabalho foi desenvolver uma plataforma digital que funcionasse como uma vitrine para os artistas locais, promovendo e valorizando suas produções."

**Objetivos Específicos:**  

1. Desenvolver um site com sistema CMS.
2. Implementar um sistema de gestão para a Escola de Artes e para Editais.
3. Criar uma vitrine digital para artistas.
4. Avaliar as funcionalidades através de testes automatizados.

**Metodologia:**  
"A execução do trabalho seguiu da seguinte maneira: Primeiro foi feita uma revisão da UML, para auxiliar na criação dos modelos de dados e dos casos de uso da plataforma, depois focou-se no desenvolvimento do sistema CMS, para a publicação de artigos e servir de base para em seguida desenvolver o sistema de gestão para a casa de cultura, envolvendo os módulos de editais, escola de artes e vitrine de artistas. Por ultimo foram realizados testes sobre o sistema para validar-lo"

---

### 4. **Revisão Bibliográfica (1 a 2 minutos)**

"As tecnologias utilizadas foram escolhidas por sua robustez e capacidade de personalização. O python foi escolhido como a linguagem de programacao principal, para agregar o frontend e o backend numa mesma linguagem, facilitando o desenvolvimento e a manutencao do codigo. Já o Django foi utilizado para auxiliar na gestão dos dados e permitir acesso direto às informações armazenadas no banco de dados, servindo como o backend da aplicacao e garantindo flexibilidade e controle durante o desenvolvimento. Essas tecnologias possibilitaram a criação de uma plataforma flexível, funcional e segura."

### LEIA O SLIDE DO WAGTAIL CRX

---

### 5. **Desenvolvimento e Implementação (13 a 16 minutos)**

**Organização do Site:**  
"O projeto foi estruturado em quatro seções principais: o site principal, a vitrine de artistas, os editais e a Escola de Artes. Cada uma dessas seções foi desenvolvida com foco em acessibilidade e usabilidade."

Apesar de na sua concepção ter desenvolvido o site principal primeiro, vou inverter a apresentação e falar dele por ultimo, apresentando primeiramente os módulos do sistema.

- **Vitrine de Artistas:**  
"O sistema permite que os artistas se cadastrem e insiram informações como nome, nome artístico, links para portfólios, fotos e vídeos.
Aqui podemos ver o diagrama ER da vitrine de artistas, envolvendo Categoria, Artista, Documento/Imagem, e as paginas do sistema Wagtail.
Esses dados são exibidos no site na vitrine de artistas, permitindo maior visibilidade aos artistas locais.(Fale mais sobre o layout, template etc.)"
Fale sobre o cadastramento, formulário incorporado no site usando o Django.
Fale sobre o papel do administrador para aprovar o artista na vitrine.

- **Editais:**  

O modelo de editais incluem informações relevantes para um edital genérico. Dados como titulo, descrição, datas e o status do edital sao gravados no banco de dados.
No diagrama ER dos editais, temos Edital, Inscrição e as paginas do sistema Wagtail.
Fale sobre o papel do administrador para aprovar as candidaturas em editais.

"A seção de editais foi criada para facilitar a submissão de propostas culturais. O sistema de editais inclui a visualização de editais abertos e fechados, permitindo aos usuários submeter suas candidaturas de forma simples e intuitiva."

(Mostre o print da página de editais e do formulário de submissão).

- **Escola de Artes:**  
"Além disso, foi criado um sistema de gestão para a Escola de Artes, que permite gerenciar turmas, alunos e professores.

Fale modelo de dados

Fale funções professor, aluno.

O administrador pode acompanhar a frequência e o desempenho dos alunos, melhorando a organização da escola."

(Mostre o print da página de gerenciamento da Escola de Artes).

- **Site principal:**  
 (Mostre os prints das páginas.)

---

### 6. **Testes e Resultados (3 a 5 minutos)**

"Foram realizados quatro tipos de testes para validar a plataforma:"

- **Funcionalidade:**  
"Os testes automatizados realizados com Django validaram a criação de editais e inscrições, confirmando que a plataforma está funcionando corretamente e otimizando a gestão cultural."

- **Usabilidade:**  
"Através da ferramenta PageSpeed Insights, a plataforma recebeu uma pontuação de **100 em acessibilidade móvel** e **97 em desktop**, com apenas uma observação sobre o contraste de um botão."

- **Desempenho:**  
"O GTmetrix avaliou a performance da plataforma em **90%**, mesmo em condições adversas de hospedagem. Com a futura migração para a infraestrutura da prefeitura, o desempenho será ainda melhor."

- **Segurança:**  
"As ferramentas Pentest Tools e Immuniweb avaliaram a segurança do site. Foram identificados apenas problemas de baixo nível, e o sistema recebeu a nota **A-** no quesito segurança, demonstrando que a plataforma foi desenvolvida com práticas robustas de proteção de dados."

---

### ** PONTOS NEGATIVOS **
EXPLICAR PORQUE NAO FOI POSSIVEL REUNIR COM A CASA DE CULTURA (TEMPO, ATAREFADOS, CONTATO DIFICIL)

### 7. **Conclusão (1 minuto)**

"O desenvolvimento da plataforma de artistas monlevadenses atingiu os objetivos propostos. Foi criado um ambiente digital que amplia a visibilidade dos artistas locais, oferece um sistema eficiente de gestão cultural e facilita a divulgação de editais e eventos culturais."

---

### 8. **Trabalhos Futuros (1 minuto)**

"Entre os próximos passos, estão a implantação da plataforma na Casa de Cultura com a infraestrutura adequada e a inclusão de novas funcionalidades, como:

1. Algoritmos de recomendação para melhorar a experiência do usuário.
2. Acessibilidade aprimorada com leitores de tela e comandos de voz.
3. Criação de um marketplace para que os artistas possam vender suas obras diretamente pela plataforma."

---

### 9. **Agradecimentos e Perguntas (1 minuto)**

"Agradeço mais uma vez à banca por toda a atenção. Estou à disposição para responder quaisquer perguntas."
