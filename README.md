# SENHA

<?php
require "conexao.php";

$nome = 'loucosporti;
$email = 'loucosporti@gmail.com.com.br';
$senha = password_hash('loucos1234', PASSWORD_DEFAULT);


$conexao = conexao::getInstance();
$sql = "INSERT INTO tab_usuario(nome, email, senha, status)VALUES('{$nome}', '{$email}', '{$senha}', 'Ativo')";
$stm = $conexao->prepare($sql);
$stm->execute();
1
2
3
4
5
6
7
8
9
10
11
12
<?php
require "conexao.php";
 
$nome = 'loucosporti;
$email = 'loucosporti@gmail.com.br';
$senha = password_hash('loucos1234', PASSWORD_DEFAULT);
 
 
$conexao = conexao::getInstance();
$sql = "INSERT INTO tab_usuario(nome, email, senha, status)VALUES('{$nome}', '{$email}', '{$senha}', 'Ativo')";
$stm = $conexao->prepare($sql);
$stm->execute();
