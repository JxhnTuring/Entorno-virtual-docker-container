<h1>Crear contenedores con imagen nodejs</h1>
<ul>
  <li>Crear el contenedor para el cliente</li>
  <code>docker run -it --name client -v ${PWD}/tudu-client:/app -w /app -p 5173:5173 node:20 bash</code>
  <li>Crear el contenedor para el server</li>
  <code>docker run -it --name server -v ${PWD}/tudu-server:/app -w /app -p 8080:8080 node:20 bash</code>
  <li>Para abrir los contenedores despues de apagados</li>
  <code>docker start -ai nombre-container</code>
</ul>
