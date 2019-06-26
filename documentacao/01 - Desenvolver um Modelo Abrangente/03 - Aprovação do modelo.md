# Aprovação do modelo base

O cliente enviou um documeto descrevendo as alterações necessárias, logo não será necessário um documento de aprovação, pois isto já comprova as alterações que devem ser desenvolvidas pela equipe.

Documento enviado pelo cliente:

```
T7 - Primeiro cliente
Parabéns!!!!

Sua organização conquistou o primeiro cliente.

Segue a exigência do cliente com relação ao produto:

"Não consigo entender esta interface, não há nenhuma indicação dos campos. O que este botão faz?"

Coloque rótulo nos campos indicando "código" e "nome" e também no botão, indicando-o como "salvar".

Execute totalmente seu processo, construa toda documentação necessária, indicada em seu processo.

No final da execução desta tarefa, sua equipe deverá ser capaz de comprovar por meio de documentos:

a) Quem modificou o código fonte do aplicativo (incluindo criação de script sql);

b) Quando o código fonte foi modificado (incluindo criação de script sql);

c) Quando e quem criou o banco de dados e tabelas no servidor;

d) Onde as senhas (do servidor e do banco de dados) estão armazenadas e quem tem acesso a elas;

e) Quem efetuou o deploy do aplicativo no servidor;

f) Quando foi efetuado o deploy no servidor;

g) Se a baseline foi atualizada ou foi criada uma nova distribuição;

h) Onde estão os documentos deste cliente (especificação de requisitos, etc..);

Nesta atividade você deverá efetuar o deploy "/cli1" no servidor e entregar uma nova versão do processo no formato .war (se necessário). Utilize split para dividir o arquivo caso necessite.

Configure o crontab para que o payara seja carregado após inicialização do computador. Edite a última linha do crontab com o comando:

#crontab -e

Irá aparecer 3 opções de editores de texto, o nano é o mais fácil.

Crie uma última linha no arquivo  com a seguinte sintaxe:

@reboot <caminho do java>/java -jar <payara-micro .jar> <arquivo1.war, arquivo2.war... arquivon.war> --addjars <bibliotecas java - jdbc>

Possivelmente a linha ficará semelhante a esta:

@reboot /usr/bin/java -jar payara-micro-5.191.jar cli1.war --addjars postgresjdbc.jar

Verifique se a rotina está funcionando com o comando #sudo init 6 para reiniciar o computador

Os endereços dos servidores são:

10.20.19.7 - grupo1
10.20.19.8 - grupo2
10.20.19.9 - grupo3
10.20.19.10 - grupo4
```