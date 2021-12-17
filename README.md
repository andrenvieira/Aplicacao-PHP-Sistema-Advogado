# Aplicação PHP para o Advogado

Requisitos para o funcionamento do script:
Não tem como garantir o funcionamento fora desses requisitos abaixo:

<h4> Servidor Linux com cPanel da (cpanel.net)
 PHP 5.4, 5.5, 5.6
 MySQL
 Apache
 phpMyAdmin</h4>

<h4>Configuração do banco de dados:</h4>
<p>Acesse o cPanel - No gerenciador de Banco de dados MySQL, crie o Banco de Dados MySQL, o
Usuário de acesso ao banco + senha, depois atribua todas as permissões do usuário ao Banco.
Nos arquivos do script que estão dentro da pasta /script acesse o seguinte arquivo e edite conforme
os dados do banco mysql que criou anteriormente.
Abrir o arquivo /application/config/database.php</p>
<p>Linhas 50 - 54
Alterar os dados conforme seu servidor:
$db['default']['hostname'] = 'localhost'; //Geralmente é localhost mesmo
$db['default']['username'] = 'USUARIOCPANEL_USUARIOBANCO';
$db['default']['password'] = 'SENHA';
$db['default']['database'] = 'USUARIOCPANEL_BANCO';
$db['default']['dbdriver'] = 'mysqli';
Importar a base de dados que está dentro da pasta /INSTALACAO
- Importe pelo phpmyadmin a base de dados BANCO-DE-DADOS.sql que está dentro da pasta
/INSTALACAO para o banco que criou pelo MySQL.</p>
<h4>Enviando os Arquivos:</h4>

<p>Agora compacte o conteúdo da pasta /Script em um arquivo .zip e faça o upload deste arquivo
zipado pelo Gerenciador de Arquivos do cPanel e assim que finalizar o upload descompacte o .zip lá
 pelo gerenciador mesmo. Obs: Verifique se está enviando o .htaccess junto. </p>

<h4>Área Administrativa:</h4>
<p>Acesse www.seusite.com.br/admin ou www.seusite.com.br/PASTA/admin
Usuário padrão: admin
Senha padrão: 123456
Altere a senha após acessar o painel do sistema.
 App  ainda em desenvolvimento, está livre para download, para qualquer DEV, efetuar alterações.</p>
