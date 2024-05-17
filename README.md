# Password Hunter info
### Descripción del funcionamiento de la aplicación Password Hunter

Es una aplicación CLI que vulnera cuentas de Instagram y Facebook. Mediante web scraping, recolecta información pública en la web sobre cada usuario y con estos datos genera contraseñas únicas para cada user, siguiendo un patrón. Luego, itera cada cuenta probando las contraseñas generadas hasta que logra acceder. Implementa un sistema de aviso por email a los usuarios cuyas cuentas fueron vulneradas, para alertarlos de posibles hackeos maliciosos. 

<br></br>
<br></br>

<div align="center">
  <img src="https://github.com/G4s70n/Password_Hunter_info-/assets/93175088/17ea87c9-6cc6-419b-9e73-918bd23b86a3" alt="publi2" style="width:60%;">
</div>
<br></br>

# ¿CÓMO FUNCIONA?
<br></br>

⚙️ Extrae información de usuarios de grupos de Facebook o seguidores/seguidos de una cuenta de Instagram que se le indique.
<br></br>

⚙️ Procesa y aloja toda esa información en una base de datos.
<br></br>

⚙️ Busca información en Internet sobre los usuarios recopilados y con base en esa info, genera contraseñas únicas para cada user, usando un patrón.
<br></br>

⚙️ Intenta loguearse con todos los usuarios a los cuáles se les generó una contraseña.
<br></br>


⚙️ Cuando accede a una cuenta, puede extraer toda su información:
<br></br>

<div align="center">
  <img src="https://github.com/G4s70n/Password_Hunter_info-/assets/93175088/3f3ba465-e24e-4f9c-aba8-a96d26e43e72" alt="publi2" style="width:60%;">
</div>
<br></br>

Esta funcionalidad, es solo para demostrar la capacidad que puede tener. Su verdadera intencionalidad está en esta siguiente funcionalidad:

⚙️ Envía un correo a todos los emails que la cuenta tenga asociados, para advertirle al usuario que su cuenta ha sido vulnerada y que aumente la seguridad de la misma para evitar hackeos maliciosos.
<br></br>

<div align="center">
  <img src="https://github.com/G4s70n/Password_Hunter_info-/assets/93175088/71b6cb47-d0b1-4c74-bdde-d8250fef9ff1" alt="publi2" style="width:60%;">
</div>

<br></br>
<br></br>


Para poner un ejemplo general del funcionamiento, tomemos 1 millón de usuarios e intentemos acceder a sus cuentas con la contraseña "L-gante" (nombre de un cantante). Probablemente, fallaremos 1 millón de veces intentando acceder a una cuenta. Sin embargo, si segmentamos a esos usuarios y tomamos 1 millón de usuarios de Argentina, de entre 15 y 25 años (mayoritariamente la edad del público que consume a ese artista), es probable que logremos acceder a varias cuentas. Es factible que dentro de ese millón de personas, algunas hayan usado el nombre de su artista favorito como contraseña. Esto es un patrón, así cómo este puede haber varios. Esta aplicación explota un patrón que la gente suele usar a la hora de crear contraseñas, que lograr hallarlo me tomó cientos de intentos fallidos.

<br></br>
<br></br>

La aplicación fue creada con fines de aprendizaje e investigación, y considerando el daño que podría causar su mal uso, he decidido no hacer público el código.
<br></br>
<br></br>

#### Tecnologías usadas:
JavaScript | Playwright | Node.js | Sequelize | PostgreSQL


