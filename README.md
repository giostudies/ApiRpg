1. Como gerar token:
http://localhost:5104/usuarios/Autenticar
 No postman, selecionar POST. Ir em body, selecionar RAW e selecionar JSON ao lado.
 No corpo do json, colocar:
 
 {
    "Username":"Usuario2",
    "Password": "123456"
}

2.Como registrar novo usuario:
  http://localhost:5104/Usuarios/Registrar
  Body > raw > Json
  
  {
    "Username":"Usuario2",
    "Password": "123456"
}
   

3. Como usar o metódo getbyperfil:
   http://localhost:5104/Personagens/GetByPerfil/1
   Em headers, na key colocar "Authorization" e em VALUE Colocar "BEARER + Seu token gerado"

Banco de dados:

Lembrete:
Para subir um script que esteja no código, copiar o script (como por exemplo, o script06) e subir diretamente pelo SQL, na tabela que tiver subido com dotnet new ef data base update.

Ao criar um novo usuário, ir direto no banco de dados, clicar com o direito na tabela usuarios, e em edit 200 rows, adicionar o tipo de perfil daquele usuario (Admin ou Jogador)

