                Cenários para testes
  1. testes de recuperação de informações de um personagem:
    • Fazer uma requisição GET para ‘/people/{id}/’ para obter informações de um personagem
      específico.
    • Verificar se o código de resposta de status é 200 (ok)
    • Verificar se as informações retornadas correspondem aos dados esperados
  
  2. testes de recuperação de lista de personagens:
    • Fazer uma requisição de GET para ‘/people’ para obter a lista de personagens.
    • Ver Verificar se o código de resposta de status é 200 (ok)
    • Verificar se a resposta contém uma lista de personagens.
    • Verificar se a paginação está funcionando corretamente dando GET ‘/people/?page=1’
  
  3. testes de recuperação de filmes associados a um personagem:
    • Fazer uma requisição GET para /people/{id} para obter as informações de um personagem
    específico.
    • Verificar se o código de resposta é 200 (OK).
    • Verificar se a lista de filmes associados ao personagem contém URLs válidas.
    • Fazer uma requisição GET para cada URL de filme retornado e verificar se os dados do filme
    são retornados corretamente.
  
  4. Teste de recuperação de espécies associadas a um personagem:
    • Fazer uma requisição GET para /people/{id} para obter as informações de um personagem
      específico.
    • Verificar se o código de resposta é 200 (OK).
    • Verificar se a lista de espécies associadas ao personagem contém URLs válidas.
    • Fazer uma requisição GET para cada URL de espécie retornado e verificar se os dados da
      espécie são retornados corretamente.
  
  5. Teste de recuperação de veículos associados a um personagem:
     • Fazer uma requisição GET para /people/{id} para obter as informações de um personagem
    específico.
     • Verificar se o código de resposta é 200 (OK).
     • Verificar se a lista de veículos associados ao personagem contém URLs válidas.
     • Fazer uma requisição GET para cada URL de veículo retornado e verificar se os dados do
       veículo são retornados corretamente.
  
  6. Teste de recuperação de espaçonaves associadas a um personagem:
    • Fazer uma requisição GET para /people/{id} para obter as informações de um personagem
      específico.
    • Verificar se o código de resposta é 200 (OK).
    • Verificar se a lista de espaçonaves associadas ao personagem contém URLs válidas.
    • Fazer uma requisição GET para cada URL de espaçonave retornado e verificar se os dados da
      espaçonave são retornados corretamente.
  
  7. Teste de limite de entrada inválido:
    • Fazer uma requisição GET para /people/{id} com um ID inválido ou inexistente.
    • Verificar se o código de resposta é 404 (Not Found) ou 400 (Bad Request) dependendo da
     implementação da API.

                     Relatorios de Bugs/Falhas
   1.Personagem: Luke Skywalker;
           • Dado que eu faço uma requisição GET para o ID 1,
           • Então o resultado deverá ser status 200,
           • E o body deverá conter as infiltrações esperadas do ID 1,
           • O teste foi concedido com sucesso.
   
   2.Personagem: C-3PO;
           • Dado que eu faço uma requisição GET para o ID 2,
           • Então o resultado deverá ser status 200,
           • E o body deverá conter as infiltrações esperadas do ID 2,
           • O teste foi concedido com sucesso.
   
   3.Personagem: R2-D2;
           • Dado que eu faço uma requisição GET para o ID 3,
           • Então o resultado deverá ser status 200,
           • E o body deverá conter as infiltrações esperadas do ID 3,
           • O teste falha pois no item films está com link errado.
   
   4.Personagem: Dart Vader;
           • Dado que eu faço uma requisição GET para o ID 4,
           • Então o resultado deverá ser status 200,
           • E o body deverá conter as infiltrações esperadas do ID 4,
           • O teste foi concedido com sucesso.
   
   5.Personagem: Leia Organa;
           • Dado que eu faço uma requisição GET para o ID 5,
           • Então o resultado deverá ser status 200,
           • E o body deverá conter as infiltrações esperadas do ID 5,
           • O teste falha pois no item created está com link errado.
   
   6.Personagem: Owen Lars;
           • Dado que eu faço uma requisição GET para o ID 6,
           • Então o resultado deverá ser status 200,
           • E o body deverá conter as infiltrações esperadas do ID 6,
           • O teste foi concedido com sucesso.
   
   7.Personagem: Beru Whitesun lars;
           • Dado que eu faço uma requisição GET para o ID 7,
           • Então o resultado deverá ser status 200,
           • E o body deverá conter as infiltrações esperadas do ID 7,
           • O teste falha pois no item films está com link errado.
   
   8.Personagem: R5-D4;
           • Dado que eu faço uma requisição GET para o ID 8,
           • Então o resultado deverá ser status 200,
           • E o body deverá conter as infiltrações esperadas do ID 8,
           • O teste falha pois no item films, species e created está com link errado.
    
   9.Personagem: R5-D4;
           • Dado que eu faço uma requisição GET para o ID 8,
           • Então o resultado deverá ser status 200,
           • E o body deverá conter as infiltrações esperadas do ID 8,
           • O teste foi concedido com sucesso.    

        
