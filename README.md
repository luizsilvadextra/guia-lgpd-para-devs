# Guia LGPD para devs
Este é um guia rápido e objetivo com pontos que devem ser considerados na definição e desenvolvimento de software levando em conta a LGPD (ou GDPR que é base da LGPD).

### O que é LGPD
A Lei Geral de Proteção de Dados é a lei brasileira baseada na européia GDPR. Esta lei destina-se a proteger e garantir a privacidade das pessoas que utilizam qualquer software.

### O que é a GDPR
A LGPD não é clara em alguns pontos. Por isso a GDPR é usada como referência. Ela é a lei europeia com mais de 200 páginas detalhando o que pode e o que não ser feito com informações pessoais e é precursora nesse sentido. Detalhe importante: mesmo fora da europa um sistema está sujeito à GDPR quando contem dados de pessoas europeias.

`O Regulamento Geral sobre a Proteção de Dados 2016/679 é um regulamento do direito europeu sobre privacidade e proteção de dados pessoais, aplicável a todos os indivíduos na União Europeia e Espaço Económico Europeu que foi criado em 2018. Regulamenta também a exportação de dados pessoais para fora da UE e EEE.`

- https://pt.wikipedia.org/wiki/Lei_Geral_de_Prote%C3%A7%C3%A3o_de_Dados_Pessoais
- https://gdpr-info.eu/art-6-gdpr/
- http://www.planalto.gov.br/ccivil_03/_ato2015-2018/2018/lei/L13709.htm

# Direto ao Ponto - o que muda??
Os pontos chave da mudança são os seguintes:
- Dados de uma pessoa não devem ser solicitados sem um bom motivo pra isso
- Havendo um bom motivo o usuário deve ser avisado deste motivo. Essa justificativa deve estar clara
- Aceitar compartilhar os dados não deve ser a opção padrão do usuário
- Mesmo que uma pessoa aceite compartilhar seus dados ela deve conseguir enxergar quais dados a empresa possui sobre ela
- Sabendo quais dados, a pessoa deve saber também qual a fonte das informações sobre ela
- É necessário saber quando ela aceitou compartilhar seus dados
- Uma vez que a empresa tem dados da pessoa, deve ser possível que a pessoa revogue o acesso a seus dados. Nesse caso a empresa deve apagar as informações da pessoa de seus sistemas
- Informações que possam identificar a pessoa (como IP, geolocalização, ou qualquer forma de identificação por comportamento) podem ser consideradas na lei, mas isto não está claro ainda.
- Metodos de cálculo considerando informações da pessoa podem ser expostos (exemplo: score financeiro)
- Se as informações da pessoa forem compartilhadas com outros sistemas ela deve ser informado sobre isso
- A pessoa é dona de suas informações.


## Exemplos práticos
1 - Um cliente quer uma página de cadastro com Nome, CPF, Email e Endereço da pessoa para um sistema de notícias online.
- Entendendo que o email é uma identificação única válida para a pessoa, qual a necessidade do CPF?
- Entendendo que o sistema de notícias não faz diferença de localização, qual a necessidade do Endereço?

*Justificativa válida:* o sistema faz publicidade baseada no endereço da pessoa e essa é a forma como ele ganha dinheiro (caso The Guardian (https://www.theguardian.com/uk).

*Não justificado:* CPF - seria válido se houvesse uma validação se a pessoa é uma pessoa real (junto à receita federal por exemplo)

*Justificativa inválida:* No futuro pode ser que precisemos do endereço para enviar uma correspondencia física à pessoa. Se for o caso pode haver um formulário com preenchimento opcional e com justificativa clara.



