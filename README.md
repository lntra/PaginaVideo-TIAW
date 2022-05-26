# Página Vídeo TIAW
O 
Sprint 2 da matéria de TIAW, o artefato em que este projeto foi montado é **Dinâmica com Javascript**

## Página do projeto
Esta é a página com a dinâmica javascript, e ela é a única. 
Não foi determinado um tema de aula definido para a página, ela foi pensada para ser um template genérico para diversos cursos da página Codeflix.

![chrome_qUq2w8m0Tx](https://user-images.githubusercontent.com/97913564/170512716-f4d5c497-52b2-433c-824f-d0ad2c8aa261.png)
![chrome_6l20g2gwrH](https://user-images.githubusercontent.com/97913564/170513079-4d661abf-7ea0-4621-8b43-733b2616c345.png)

Foi implementado com o html e css, a seção estática da página, tanto uma seção de vídeo Iframe, quanto uma parte destinada aos materiais usados no curso e uma 
seção de comentários.

Todos os componentes utilizados no projeto, como o Iframe do youtube é apenas usado de preenchimento e não tem correlação com o que seria utilizado no 
modelo final com a implementação dos cursos.

## Descrição das Dinâmicas Javascript
### Botão baixar Todos
![chrome_rMYe8rlOW0](https://user-images.githubusercontent.com/97913564/170519890-cf589530-a6f6-4155-88e9-340f17d090e6.png)

Este botão baixa todo material posteriormente colocado na página do curso, ao invés de ter que clicar individualmente cada um.
### Curtida
![chrome_YDOnw31ikC](https://user-images.githubusercontent.com/97913564/170519574-fe97a428-c795-47c5-8baf-26d765f72814.png)

A curtida é uma ferramenta de avaliar os comentáirios que não sejam os próprios, quando um comentário é curtido o svg do coração é alterado para a cor padrão do site
### Teste 1 - O botão já foi marcado?
O primeiro teste deste componente de curtida é testar se o botão já foi clicado pelo usuário.

***Pré condições:*** O js está funcional

***Ações***
1. Acessar a página
    - Clicar no botão de curtida de algum comentário
     - Trocar variável de false para true e vice-versa paras próximas operações no mesmo botão
        - Ao  mesmo tempo trocar a contagem no html do site
      - Adicionar uma classe de estilo css

***Resultados Esperados***

Ao apertar no coração o número de curtidas subirá em 1 e a condição de execução será alterada, e o estilo do coração alterará para um na cor padrão do site.

### Comentar
![chrome_JiHuyXbtpg](https://user-images.githubusercontent.com/97913564/170519754-027bcb16-1874-4715-8609-76b15dfc15f8.png)

A seção de comentar é composta por um input de texto e um botão de ***Publicar***	 e este publica as mensagens que o usuário do site desejar.
### Teste 2 - Comentário OK
O segunto teste faz a avaliação do conteúdo do comentário e conclui publicando no site.

***Pré condições:*** O js está funcional

***Ações***
1. Acessar a página
   - Digitar um comentário no input
    - Clicar no botão de publicar
     - Analisar o Input do form
      - Publicar no site

***Resultados Esperados***

Após digitar, ao clicar no botão, o comentário aparecerá embaixo dos outros padrões, mas não poderá ser curtido pelo próprio usuário.

### Teste 3 - Comentário NÃO OK
O terceiro teste faz a avaliação do conteúdo do comentário e conclui descartando o comentário

***Pré condições:*** O js está funcional e o comentário está vazio

***Ações***
1. Acessar a página
    - Clicar no botão de publicar
     - Analisar o Input do form
       - Não publicar no site

***Resultados Esperados***

Após digitar, ao clicar no botão, o comentário ***Não*** aparecerá embaixo dos outros padrões por estar sem conteúdo dentro, não permitindo a formação de comentário
mas não poderá ser curtido pelo próprio usuário.
