# SeparadorDeEmails

## Introdução
Trabalho final da matéria Inteligência Artificial da turma 2026.1 da Faculdade IBMR.
O objetivo do trabalho foi escrever um código com o básico do Python que pudesse reconhecer e-mails considerados Spam e separa-los de um grupo de e-mails.

Para criar este código utilizei somente ate a estrutura de dados Lista para realizar a manipulação de dados, também para praticar usei a manipulação de arquivos.

Para ele realizar seu objetivo o programa precisa de dois arquivos de texto, um deles contem os e-mails e no outro os termos para identificar quais seriam os e-mails indesejáveis.

Cada e-mail ocupa uma linha do arquivo e é composto primeiro pelo endereço do e-mail e depois separado por espaço o conteúdo do e-mail.

Para armazenar os e-mails spam e os normais foi usado listas, uma contendo os endereços de e-mails considerados suspeitos e outra com os normais.

O programa passa por cada e-mail, primeiro vê em que categoria se encontra o endereço, caso o endereço já esteja em uma das listas o e-mail já é transferido para sua respectiva categoria.

Já caso o endereço ainda não esteja armazenado em nenhum lugar o programa passa pelo conteúdo do e-mail a procura de algum dos termos do arquivo de termos, caso tenha algum dos termos proibidos ele guarda o endereço de e-mail na lista dos endereços Spam, se não tiver ele vai para a lista de e-mails normais.

Mas o mesmo endereço suspeito pode ter mandado vários e-mails diferentes, e é ai que o programa realiza sua função principal.

## Funcionamento

### Menu

Ao iniciar o programa usuário tem 5 opções para interagir com o código:
- Visualizar todos os e-mails
- Mudar um e-mail de lugar
- Criar os arquivos das caixas atualizadas
- Atualizar todos os e-mails
- Sair do programa

**IMAGEM1**

### Funcionalidades

Funcionalidade criada para cumprir o requisito do trabalho:
 - Visualizar todos os e-mails existentes, já separados entre Caixa de Entrada e a Caixa de Spam.
   
Funcionalidades extras:
- Coloquei a possibilidade do usuário mudar o e-mail de lugar (Da caixa de entrada para caixa de Spam ou vice versa).
- Atualizar as duas caixas de e-mails, já que ao mudar os e-mails de lugar os endereços também mudam de estado (entre endereço normal e suspeito)
- Criar dois arquivos com os e-mails separados, um com os da caixa de entrada, que são os e-mails normais, e outro com os da caixa de Spam, os e-mails suspeitos.

### Visualização dos E-mails
A visualização dos e-mails no terminal seguiram como duas listas já separadas entre e-mails normais e e-mails spam, os e-mails seguem a ordem que está no arquivo de e-mails.

**IMAGEM2**

### Mudar o e-mail de lugar
Mudar o e-mail de lugar significa que ele mudará para a outra categoria automaticamente, ou seja, se ele estava na caixa de entrada ele mudará para caixa de spam e caso ele estava na caixa de Spam ele mudará para caixa de entrada. 

Além disso o endereço também mudará seu estado de não suspeito para suspeito ou de suspeito para não suspeito, respectivamente.

Mas naquele momento somente aquele e-mail irá mudar de categoria, os outros e-mails ainda estarão em suas respectivas categorias, ate que o usuário aperte para atualizar todos os e-mails, assim realocando todos os e-mails de endereços normais na caixa de entrada e os e-mails de endereço suspeito na caixa de spam. 

Primeiro opta em quais das 2 caixas.

 **IMAGEM3**
 
 E depois por qual e-mail dela.
 
 **IMAGEM4**

### Criar os arquivos das caixas atualizadas
Ao selecionar esta opção o programa criará 2 arquivos de texto na mesma pasta chamados emails_nomais e emails_spams, um com os da caixa de entrada, que são os e-mails normais, e outro com os da caixa de Spam, os e-mails suspeitos respectivamente. 

Eles estarão separados da posição em que os e-mails se encontram no momento em que a opção foi selecionada, mas caso o usuário mude os e-mails de categoria, os atualize e selecione esta opção novamente o programa somente irá atualizar os dois arquivos já criados anteriormente. 

*Obs.: Apesar do nome da funcionalidade não fica criando diversos arquivos diferentes.*

**IMAGEM5**

## Considerações finais
Eu achei um bom trabalho para introduzir ao Python de uma forma mais desafiadora, dado o tempo e o conhecimento limitado na época que foi criado acabou que muitas das melhorias que precisariam para aperfeiçoar o projeto acabaram não entrando no projeto finalizado, entre elas:

- Melhorar a visualização dos e-mails para uma visualização mais limpa e ampla, uma opção seria de ao iniciar o programa já haver dois arquivos com já os e-mails separados, de vez de só mostra-los no terminal, assim a visualização ficaria mais "próxima" ao usuário.
- Colocar a opção de adicionar novos e-mails ou excluir e-mails existentes.
- Colocar a opção de adicionar novos termos ou excluir termos existentes.
- Deixar a execução mais eficiente e analisar se no próprio endereço tem informações suspeitas.
- Conseguir analisar e-mails mais complexos ou escrito de outros formatos.
- Melhorar a forma que o programa separa entre e-mails suspeitos ou não.

Ainda daria para melhorar de inúmeras formas além dessas, mas como o objetivo do projeto era para ser uma introdução ao Python, uma complexidade bem maior sairia do objetivo.


## Notas
Este projeto foi finalizado em junho de 2026 e na época foi inicialmente publicado para correção com o nome [RastreadoOSpam](https://github.com/Ariproductor/RastreadoOSpam). Este novo repositório é um repositório para oficializar o projeto e dá sua conclusão.





