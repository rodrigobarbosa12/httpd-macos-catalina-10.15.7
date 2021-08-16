
## 🏗 Alterações no arquivo httpd.conf

### 1º Passo
    User _www
    Group _www

    para

    User username
    Group _www

### 2º Passo
    Options FollowSymLinks Multiviews

    para 

    Options FollowSymLinks Multiviews Indexes

### 3º Passo
    DocumentRoot "/Library/WebServer/Documents"
    <Directory "/Library/WebServer/Documents">

    para 

    DocumentRoot "/Users/username/Sites/"
    <Directory "/Users/username/Sites/">

### 4º Passo
    # Virtual hosts

    #Include /private/etc/apache2/extra/httpd-vhosts.conf

    para

    Include /private/etc/apache2/extra/httpd-vhosts.conf
    Ou 
    Include /private/etc/apache2/users/*.conf // Personalizavel

#### 5º Passo
    restart apache2

## Autor

<a href="https://www.linkedin.com/in/rodrigo-barbosa-7a1429157/">
 <sub>
    <b>Rodrigo Barbosa</b>
 </sub>
</a>
<a href="#" title="Rocket">🚀</a>

 <br />
 <br />

[![Github Badge](https://img.shields.io/github/followers/rodrigobarbosa12?style=social&link=https://github.com/rodrigobarbosa12)](https://github.com/rodrigobarbosa12)

<Feito com 💙 />
