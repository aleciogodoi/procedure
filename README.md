<h1>Pitch Class FIAP</h1>

Alécio Aparecido Preto de Godoi</br>   
Tema: Procedure em Banco de Dados</br>
Vídeo https://youtu.be/yzBwwJr-hBo

<h2>Script Tabela Produto</h2>


Utilizar o SQLiteOnLine: <a href="https://www.w3schools.com">https://sqlliteonline</a>
<em>
</br></br>
Create Table Produto (</br>
  codigo int identity,</br>
  nome varchar(100),</br>
  qtde int,</br>
  preco decimal(8,2)</br>
  );</br>
</em>

<h2>Script Procedure ProdutoIncluir</h2>
<em>
Create Procedure ProdutoIncluir </br>
   @nome varchar(100), @qtde int, @preco decimal(8,2) </br>
AS </br>
Insert Into Produto (nome, qtde, preco) VALUES (@nome, @qtde, @preco) </br>
</em>

<h2>Incluindo Produto</h2>
<em>
execute ProdutoIncluir 'Motorola G 100', 10, 2956.32; </br>
</em>

<h2>Consultando Produto</h2>
<em>
Select * From Produto;
</em>
