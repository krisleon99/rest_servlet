# rest_servlet


1. Servicios REST desarrollado en JAVA 9

# Es un servicio que acepta solicitudes HTTP GET en:

http://localhost:8080/greeting/RestServlet

# responde con una representación JSON de un saludo:

{​ "id"​ : ​ 1 ​ , ​ "content"​ : ​ "Hello, World!"​ }

Cuenta con un saludo personalizado con un parámetro de nombre opcional en la cadena de
consulta:

http://localhost:8080/greeting/RestServlet?user=User

dejando como respuesta  respuesta:
{​ "id"​ : ​ 1 ​ , ​ "content"​ : ​ "Hello, User!"​ }

IDE utilizado: Eclipse

Instalaciones adicionales: JDK y JRE

# Windows

sitio de descarga:

https://www.oracle.com/technetwork/es/java/javase/downloads/index.html

# Linux

sudo apt install openjdk-9-jdk

#gson-2.2

Para enviar una respuesta JSON desde el Servlet, primero tenemos que convertir el objeto LinkedHashMap en su representación JSON. usamos: gson-2.2.2.jar
lo ponemos el jar en la carpeta lib de WebContent

sitio de descarga:

http://www.java2s.com/Code/Jar/g/Downloadgson222jar.htm

#necesitamos un servidor, en este caso se ocupo apache Tomcat v9

sitio de descarga:

http://tomcat.apache.org/

En caso de Windows:

Se descomprime el archivo, luego vamos a renombrar la carpeta como “tomcat” y la pegaremos en el disco C:\

#tenemos que configurar las variables de entorno JAVA_HOME 

#para correr tomcat nos posicionamos en la carpeta tomcat:

.\bin\startup.bat

#para parar tomcat nos posicionamos en la carpeta tomcat:

.\bin\shutdown.bat
