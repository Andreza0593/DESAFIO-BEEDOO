# Desafio de QA Beedoo

## User Story: Formulário de Cadastro de Curso

Como **administrador de curso**, eu quero **cadastrar um curso** para que **ele possa ser listado e acessado por potenciais estudantes**.

### Critérios de Aceitação:
1. O formulário deve incluir campos para:
    - Nome do Curso (campo de texto)
    - Descrição do Curso (área de texto)
    - Instrutor (campo de texto)
    - URL da Imagem de Capa (campo de texto)
    - Data de Início (seletor de data)
    - Data de Fim (seletor de data)
    - Número de Vagas (campo numérico)
    - Tipo de Curso (menu suspenso)
2. Cada campo deve ter validação apropriada:
    - Nome do Curso: Obrigatório
    - Descrição do Curso: Obrigatório
    - Instrutor: Obrigatório
    - URL da Imagem de Capa: Opcional, deve ser uma URL válida se fornecida
    - Data de Início: Obrigatória, deve ser uma data válida
    - Data de Fim: Obrigatória, deve ser uma data válida e não pode ser anterior à data de início
    - Número de Vagas: Obrigatório, deve ser um número inteiro positivo
    - Tipo de Curso: Obrigatório, deve ser um dos tipos predefinidos
3. Após o envio bem-sucedido, o formulário deve:
    - Salvar os detalhes do curso no banco de dados
    - Fornecer uma mensagem de sucesso ao usuário
    - Redirecionar o usuário para a página de listagem de cursos
4. Se o envio do formulário falhar, mensagens de erro apropriadas devem ser exibidas.

### Documentação das Decisões:

1. **Seleção dos Campos**: Os campos foram escolhidos com base nos requisitos típicos para o cadastro de cursos, garantindo que todos os detalhes necessários sejam capturados.
2. **Validação**: As regras de validação dos campos foram implementadas para garantir a integridade dos dados e prevenir erros durante o envio do formulário.
3. **Feedback ao Usuário**: Mensagens de sucesso e erro foram incluídas para melhorar a experiência do usuário, fornecendo um feedback claro sobre o status do envio do formulário.
4. **Redirecionamento Após Envio**: Redirecionar o usuário para a página de listagem de cursos após o envio garante que ele possa ver imediatamente o curso recém-cadastrado, melhorando a eficiência do fluxo de trabalho.
5. **URL da Imagem de Capa Opcional**: Este campo foi tornado opcional para acomodar cursos que podem não ter uma imagem de capa pronta no momento do cadastro.


### Cenários e Casos de Teste

Os cenários e casos de teste foram documentados na seguinte planilha do Google Docs:

[Link para a Planilha de Casos de Teste](https://docs.google.com/spreadsheets/d/14Je_anZR_5CTuB_8II4rlKGbgoi3i_cJEZMoeFrZCx0/edit?gid=0#gid=0)

