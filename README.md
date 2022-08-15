# metapol-app Installation

<h3> Place all files to the root folder, then move all files in public folder to your website public_html or www directory.</h3>

<h4> Requiremens</h4>

 // FOLDER PLACEMENT // <br>
    |---root <br>
    |---|---metapol_app <br>
    |---|---public (or public_html) <br>
    |---|---|---index.php <br>

<h3><strong>Please Note:</strong>The 'metapol_app' and 'public' folder are siblings.</h3

- metapol_app/storage/framework/        # 775<br>
- metapol_app/storage/logs/             # 775<br>
- metapol_app/storage/app/kyc-files/    # 775<br>
- metapol_app/storage/app/public/       # 775<br>
- metapol_app/bootstrap/cache/          # 775<br>

<h4>You must set these folders; framework, logs, kyc-files, cache permission to 775 as above. Sometimes based on server permission 775 may not work, then you have to set 777</h4>

<h3>Before starting the installation process please confirm server requirements as below.</h3>

<li> - PHP >= 7.3 (support upto 7.4)
<li> - OpenSSL PHP Extension
<li> - PDO PHP Extension
<li> - Mbstring PHP Extension
<li> - Tokenizer PHP Extension
<li> - XML PHP Extension
<li> - Ctype PHP Extension
<li> - JSON PHP Extension
<li> - BCMath PHP Extension
<li> - FileInfo PHP Extension

<h4>Manual Installation Process</h4><br>
Step One: Configure .ENV File
<h4>Go to metapol_app folder and edit the .env file.</h4>

<h4>Change these values - APP_NAME, APP_URL, DB_HOST, DB_DATABASE, DB_USERNAME, DB_PASSWORD</h4>

<pre>
<li>APP_NAME='YOUR_APP_NAME_HERE'
<li>APP_VERSION='1.0.0'
<li>APP_ENV=production
<li>APP_KEY=base64:bMzV/BygkgeonjHpn5c7NkwcAi8ckl+tBIEfNfOqgmw=
<li>APP_DEBUG=false
<li>APP_LOG_LEVEL=debug
<li>APP_URL=http://yourdomainname.com

<li>FORCE_HTTPS=false
<li>DB_CONNECTION=mysql
<li>DB_HOST=127.0.0.1
<li>DB_PORT=3306
<li>DB_DATABASE=your_db_name
<li>DB_USERNAME=your_db_user_name
<li>DB_PASSWORD=your_db_password

<li>BROADCAST_DRIVER=log
<li>CACHE_DRIVER=file
<li>SESSION_DRIVER=cookie
<li>QUEUE_DRIVER=sync

<li>REDIS_HOST=127.0.0.1
<li>REDIS_PASSWORD=null
<li>REDIS_PORT=6379

<li>MAIL_DRIVER=smtp
<li>MAIL_HOST=smtp.mailtrap.io
<li>MAIL_PORT=2525
<li>MAIL_USERNAME=null
<li>MAIL_PASSWORD=null
<li>MAIL_ENCRYPTION=null

<li>PUSHER_APP_ID=
<li>PUSHER_APP_KEY=
<li>PUSHER_APP_SECRET=</pre>
    
<h3>Step Two: Installed File placement</h3>
<li>Copy the installed file (found under manual-install-files folder) and placed into metapol_app/storage folder.

<h3>Step Three: Import Dummy SQL File</h3>
<li>Import the sql file dummy_app.sql into database.

<h4>Final Step</h4>
<h4>Once above steps are complete,go to your website url. https://your-domain.com/ & register first your Super Admin account. Then login to your account and configure the Website settings, Email settings, Payment settings and ICO Stages etc.</h4>

<h4>Note: First registered user will be always super-admin privilege.</h4>
