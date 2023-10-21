# Desafio-Processando-e-Transformando-Dados-com-Power-BI

## Descrição do Desafio
Neste projeto, o objetivo foi criar um banco de dados MySQL e hospedá-lo na plataforma Azure. Em seguida, integrar os dados com o Power BI para extrair, transformar e limpar informações relevantes. O foco final foi utilizar esses dados para criar um relatório eficaz usando as funcionalidades do Power BI.

## Descrição da Solução
Uma das etapas importantes do projeto foi mesclar os nomes de departamentos e localizações. A razão para mesclar esta na necessidade de criar uma relação única entre cada combinação de departamento e localização. Ao mesclar, é garantido que cada par de departamento e localização seja tratado como uma única entidade, facilitando a criação de um modelo estrela.

### Etapas Realizadas e Justificativas:

1. **Verificação dos Cabeçalhos e Tipos de Dados:** Antes de qualquer transformação, examinei os cabeçalhos e tipos de dados para garantir consistência e integridade dos dados.

2. **Modificação dos Valores Monetários:** Modifiquei os valores monetários para o tipo double preciso para manter a precisão das informações financeiras.

3. **Análise e Remoção dos Nulos:** Analisei os valores nulos.

4. **Verificação de Colaboradores Sem Gerente:** Identifiquei colaboradores sem gerente (coluna `Super_ssn` nula) e examinei a necessidade de preencher essas lacunas.

5. **Verificação de Departamentos Sem Gerente:** Verifiquei a existência de departamentos sem gerentes para garantir que todas as áreas da empresa estivessem adequadamente gerenciadas.

6. **Preenchimento das Lacunas:** Não foram identificados departamentos sem gerente.

7. **Verificação do Número de Horas dos Projetos:** Analisei o número de horas associadas a cada projeto para garantir consistência e validade nos dados.

8. **Separação de Colunas Complexas:** Dividi colunas complexas em partes menores para facilitar a análise e melhorar a compreensão dos dados.

9. **Mesclagem de Consultas (Employee e Departament):** Mesclei as consultas das tabelas `employee` e `departament` para criar uma tabela `employee` com os nomes dos departamentos associados aos colaboradores. A mescla foi baseada na tabela `employee` e influenciou o tipo de junção utilizada.

10. **Eliminação de Colunas Desnecessárias:** Removi as colunas que não eram relevantes para a análise, mantendo apenas as informações essenciais.

11. **Junção dos Colaboradores e seus Respectivos Gerentes:** Realizei a junção das tabelas para associar cada colaborador ao seu gerente. Isso foi feito no Power BI por meio de mesclas de tabelas.

12. **Mesclagem das Colunas de Nome e Sobrenome:** Combinei as colunas de nome e sobrenome em uma única coluna para simplificar a visualização e análise dos nomes dos colaboradores.


## Conclusão
A mesclagem adequada dos dados no Power BI é essencial para criar análises profundas e relatórios precisos. Ao entender a necessidade de combinações únicas, como no caso de departamentos e localizações, pude criar modelos eficazes e significativos para apoiar tomadas de decisões informadas. Este readme oferece uma visão geral do meu desafio e da solução, destacando a importância da mesclagem de dados no contexto do projeto.
