<h1>Agregar usuario en sistemas RHEL</h1>
Para agregar un usuario a linux se usa el comando como "sudoer":<br>
<code> useradd nombreUsuario
</code>
<br>
Sin embargo en la mayoria de distribuciones Linux no se crea su directorio <q>home</q> por lo que es mejor usar:

<code> useradd -m nombreUsuario
</code>

Una vez creado el usuario hay que asignarle una contraseña:<br>
<code> passwd nombreUsuario
</code>

<h2>Grupos de usuarios</h2>
La configuración de usuarios permite proteger al sistema y a ellos mismos 😆, para crear grupos de usuarios: <br>
<code> groupadd nombreGrupo
</code>

Y finalmente para agregar un usuario a un grupo:<br>
<code> usermod -a -G nombreGrupo nombreUsuario
</code>