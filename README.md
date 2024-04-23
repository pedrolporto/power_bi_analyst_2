# Processando e Transformando Dados com Power BI

Este repositório contém os arquivos e informações relacionadas à atividade realizada durante o curso da Digital Innovation One (DIO) sobre o Power BI.

## Screenshots
![Power BI Analyst](https://github.com/pedrolporto/power_bi_analyst_2/assets/28610184/706f1882-2f92-4dfd-bd8a-4207a1377247)

![Power BI Data Analysis](https://github.com/pedrolporto/power_bi_analyst_2/assets/28610184/a2ae5dd9-f174-458e-9e27-ab11e56f6d02)

## Passos realizados para transformação dos dados

- Alteração de nome de coluna Adress.2 para Adress_place
- Alteração de nome de coluna Adress.3 para City
- Substituição de valor na coluna Adress_place de valor Fire para Fire Oak
- Substituição de valor na coluna State de Humble para TX
- Remoção da coluna Adress.5

Mescla de tabelas ( employee | departament ) com junção das respectivas colunas Dno | Dnumber
- Nova tabela gerada com nomenclatura employee

Remoção de colunas Dno e Dnumber na tabela employee

Mescla de tabelas ( employee | employee) com junção das respectivas colunas Ssn | Super_ssn

Remoção de colunas resultantes da junção do supervisor e employee ( colunas Ssn | Super_ssn ) na tabela employee com exeção da MName ( nome do supervisor )

Alteração de nome da coluna referênte ao supervisor de MName para MNameSuper na tabela employee

Mescla de colunas Fname e Lname na tabela employee utilizando separados espaço

Alteração de nome da coluna resultante da mescla de Mesclado para Name na tabela employee

Duplicação da coluna City

Mescla de colunas City - Copiar e azure_company departament.Dname na tabela employee utilizando separador " - ". Junção nomeada como DepLocalization

Remoção das seguintes colunas na tabela employee
- azure_company departament.Mgr_start_date
- azure_company departament.Dept_create_date

Agrupamento por:
- MNameSuper
- Name
- City
- State
- Sex
- Salary
- DepLocalization

Remoção da coluna Contagem na tabela employee

## É possível a utilização de mesclar e atribuir como funções idênticas no uso comum?

É importante a noção de que os processos são distintos e servem para alteração dos dados de maneiras a possibilitar uma varidade de operações possíveis ao usuário. O comando mesclar garante a junção de informações sem a alteração do valor dos dados em questão, sendo comparáveis a manipulação de junção de strings.  No caso de Atribuir, um valor pré definido é atualizado em todos os campos, resultando em substituição das informações passíveis ao entendimento final.


## Como utilizar o arquivo do Power BI Desktop

1. **Download do arquivo**: Faça o download do arquivo `Desafio_DIO_Modulo_3.pbix` disponível neste repositório.
2. **Abra o Power BI Desktop**: Se você ainda não tiver o Power BI Desktop instalado, faça o download e a instalação a partir do [site oficial da Microsoft](https://powerbi.microsoft.com/pt-br/desktop/).
3. **Abra o arquivo**: Após abrir o Power BI Desktop, clique em "Arquivo" e selecione "Abrir" no menu suspenso. Navegue até o local onde você baixou o arquivo `.pbix` e selecione-o para abri-lo.
4. **Explorando os dados**: Agora você pode explorar as visualizações e análises presentes no arquivo. Interaja com os filtros e elementos visuais para obter insights sobre os dados.
5. **Atualização dos dados**: Se desejar atualizar os dados com novas informações, clique em "Atualizar" no Power BI Desktop para buscar os dados mais recentes da fonte original.

## Contribuições

Contribuições são bem-vindas! Se você identificar melhorias ou correções neste projeto, sinta-se à vontade para abrir uma issue ou enviar um pull request.

## Licença

Este projeto está licenciado sob os termos da [Licença MIT](LICENSE).
