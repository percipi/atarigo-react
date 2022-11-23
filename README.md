# atari go react
## Deployment
Add section in C:\xampp\apache\conf\extra\httpd-vhosts.conf:

<VirtualHost go9x9.local:80>
    DocumentRoot "C:\projekty\go9x9\dist"
    ServerName go9x9.local
	<Directory "C:\projekty\go9x9\dist">
		AllowOverride All
        Require all granted    
    </Directory>
</VirtualHost>

Add in hosts:
127.0.0.1       go9x9.local

## Run
1. Start xammp
2. npm start
