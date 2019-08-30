# GYPZ- Tech Challenge

A **DMCard** está em busca de pessoas incríveis que integrem nosso laboratório para criarmos incríveis produtos digitais, e gostaríamos de ter você aqui conosco.

Para iniciar o processo, pedimos um teste que não vai tomar muito do seu tempo e nos dará uma perspectiva da sua forma de trabalhar. Queremos entender seu nível de habilidade em todas as áreas envolvidas na construção de um projeto: **Front e Back.**

Você não precisa entregar ambos, mas qualquer adicional as suas habilidades específicas é interessante.

# Requisitos do desafio

Deve se criar uma aplicação que permitirá a solicitação de um cartão de crédito, onde o usuário irá inserir suas informações básicas e o sistema irá fazer uma análise da liberação do cartão.

Deve ser feito uma API Restful, que permitirá:

- Cartão
  - **GET**: Listará todas as solicitações de cartões no sistema.
  - **POST**: Deve inserir uma nova solicitação de cartão.
  - **DELETE**: Remove uma solicitação 

Quando o usuário solicitar um cartão, deve ter uma aprovação automática do sistema, que sua regra será:

Deverá ser criada uma rotina que verificará a pontuação de crédito do usuário que será uma rotina que devolva uma pontuação **aleatória** entre 1 a 999, para ser utilizada como score de credito.

Por exemplo:

```
import random
random.randint(1, 999)
```

Sendo que, dependendo do score retornado a solicitação é aprovada ou não, também alterando o seu limite de crédito, que deverá seguir a seguinte lógica:

| Score     | Crédito                                        |
| --------- | ---------------------------------------------- |
| 1 a 299   | Reprovado                                      |
| 300 a 599 | R$1000,00                                      |
| 600 a 799 | 50% da renda informada, valor mínimo R$1000,00 |
| 800 a 950 | 200% da renda informada                        |
| 951 a 999 | Sem limites, considerar R$ 1.000.000           |

No Front, deverá ser listado todas as solicitações, com a possibilidade da inclusão de uma nova solicitação e também possível excluir uma utilizando todos os verbos Rest disponíveis no Back.

O **Back-End** do projeto deverá ser feito em **Python ou Node.JS**, utilizando um framework de sua escolha.

O **Front-End** deverá ser feito a seu critério e justificando o porque da solução escolhida, nós achamos o React interessante.



Qualquer dúvida sobre os requisitos, você pode enviar um e-mail para mateus.vieira@dmcard.com.br



# Como fazer?

Sugerimos um prazo de 7 dias para a entrega. Caso precise de mais nos avise e Justifique.

Sobre a entrega:

- **Pedimos que você nos envie um e-mail, para sinalizar seu início no desenvolvimento do desafio.**
- Seu código deve estar disponível em um repositório no Github.
- Você pode utilizar plataformas como Heroku ou AWS para nos mostrar a aplicação funcionando em produção.
- Quando estiver pronto nos envie o link do repositório.

Boa Sorte!
