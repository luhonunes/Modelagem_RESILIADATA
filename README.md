# RESILIADATA - Projeto de Banco de Dados

Este é um projeto de banco de dados para o sistema fictício RESILIADATA, desenvolvido como parte do Módulo 3 do curso Analista de Dados da Resília Educação em parceria com o Ifood - Vamo AI. O objetivo do projeto é realizar a modelagem e posteriormente criar um banco de dados para armazenar informações sobre empresas parceiras, tecnologias, áreas e colaboradores.

## Modelagem do Banco de Dados

A seguir está a modelagem conceitual e lógica do banco de dados para o sistema RESILIADATA:
![Modelagem do Banco de Dados](https://github.com/luhonunes/Modelagem_RESILIADATA/blob/main/RESILIADATA.jpg?raw=true)

Este modelo foi criado e está disponível pelo draw.io:
[Fluxograma](https://drive.google.com/file/d/1DKdbUYS1lByDNjKKwq4Khy24UgVRCmc6/view?usp=sharing)

### Entidades e Atributos

O arquivo Excel disponível neste repositório contém a modelagem do banco de dados do sistema RESILIADATA. Ele inclui as seguintes tabelas e seus respectivos campos:

- Empresa Parceira:
  - CNPJ (chave primária)
  - Nome 
  - Endereço 
  - Telefone 
  - E-mail 
  - Área_ID (chave estrangeira referenciando a entidade Área)

- Área:
  - ID (chave primária)
  - Nome 
  - Descrição 
  - Tecnologia_ID (chave estrangeira referenciando a entidade Tecnologia)

- Tecnologia:
  - ID (chave primária)
  - Nome 
  - Descrição 
  - Área_ID (chave estrangeira referenciando a entidade Área)

- Colaborador:
  - CPF (chave primária)
  - Nome 
  - Endereço 
  - Telefone 
  - E-mail 
  - Empresa Parceira_CNPJ (chave estrangeira referenciando a entidade Empresa Parceira)
  - Área_ID (chave estrangeira referenciando a entidade Área)

### Relacionamentos

- Uma Empresa Parceira pode ter muitas Áreas (relação um para muitos).
- Uma Área pode ter muitas Tecnologias (relação um para muitos).
- Uma Tecnologia pode estar em várias Áreas (relação muitos para muitos).
- Um Colaborador pode estar em apenas uma Empresa Parceira e apenas uma Área (relação um para um).

## Exemplos de Registros

Aqui estão exemplos de registros para cada entidade:

- Empresa Parceira:
  1. CNPJ: 123456789, Nome: TechSolutions, Endereço: Rua das Inovações, 123, Telefone: (11) 1234-5678, E-mail: info@techsolutions.com, Tecnologia_ID: 1
  2. CNPJ: 987654321, Nome: DataTech, Endereço: Avenida dos Dados, 456, Telefone: (22) 9876-5432, E-mail: contact@datatech.com, Tecnologia_ID: 2

- Tecnologia:
  1. ID: 1, Nome: Phyton, Descrição: Linguagem de programação versátil e de alto nível, Área_ID: 1
  2. ID: 2, Nome: SQL, Linguagem de consulta estruturada para bancos de dados relacionais, Área_ID: 2
  3. ID: 3, Nome: Java, Descrição: Linguagem de programação orientada a objetos, Área_ID: 1

- Área:
  1. ID: 1, Nome: Webdev, Descrição: Desenvolvimento web e front-end, Tecnologia_ID: 1
  2. ID: 2, Nome: Dados, Descrição: Ciência de dados e análise de informações, Tecnologia_ID: 2

- Colaborador:
  1. CPF: 11111111111, Nome: Aldo Rabelo, Endereço: Rua das Programadoras, 789, Telefone: (11) 2323-8878, E-mail: aldinholek@email.com, Empresa_Parceira_CNPJ: 123456789, Área_ID: 2
  2. CPF: 22222222222, Nome: Mario Covas, Endereço: Avenida Fieis do Alamo, 344, Telefone: (22) 3223-9921, E-mail: covasmario@email.com, Empresa_Parceira_CNPJ: 987654321, Área_ID: 1

## Como Utilizar

1. Faça o clone deste repositório em sua máquina local.
2. Acesse o arquivo Excel para visualizar a modelagem do banco de dados.
3. Analise o fluxograma para entender a estrutura do banco de dados.
4. Utilize as informações contidas na modelagem para implementar o banco de dados no sistema.
5. As respostas das perguntas realizadas estão disponíveis no arquivo RESILIDATA.txt.

## Contribuição

Contribuições são bem-vindas! Se você encontrar algum problema ou tiver sugestões para melhorias, sinta-se à vontade para abrir uma issue neste repositório.

## Autor
Esse projeto foi desenvolvido por Luciana Otávio Nunes.

[LinkedIn](https://www.linkedin.com/in/luhonunes/)

E-mail : (lucianaotnunes@gmail.com)