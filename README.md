# Socket-Java

Creating and using sockets in Java.
<br>
The projects are created with <a href="https://netbeans.apache.org/">Netbeans</a>.
<br>
The Java source files is in the "ProjectName/Client/src/client/" and "ProjectName/Server/src/server/" directories.

<table>
  <thead>
    <tr><th>Project name</th> <th>Service offered by the server</th></tr>
  </thead>

  <tbody>
    <tr><td>001 - Uppercase string TCP</td> <td>The server converts the string sent by the client to uppercase with TCP</td></tr>
    <tr><td>002 - Uppercase string UDP</td> <td>The server converts the string sent by the client to uppercase with UDP</td></tr>
  </tbody>
</table>

URL indirizzoWeb = new URL(url);

OutputStream out;

//salva il contenuto della pagina web in un file locale del Server

InputStream in = new BufferedInputStream(indirizzoWeb.openStream());

out = new BufferedOutputStream(new FileOutputStream("C:\\Users\\url.html"));

int leggiByte;

while((leggiByte=in.read())>=0){

out.write(leggiByte);

}

in.close();

out.close();
