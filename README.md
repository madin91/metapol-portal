# metapol-portalInstallation
Unzip the Application
At first, after download the application, unzip the all files to your root folder, then move all files of public folder to your website public_html or www directory.

Requirement of Installation
    // FOLDER PLACEMENT //
    |---root
    |---|---tokenlite_app
    |---|---public (or public_html)
    |---|---|---index.php
Please Note:
Remember the 'tokenlite_app' and 'public' folder should be consider as siblings.

tokenlite_app/storage/framework/        # 775
tokenlite_app/storage/logs/                  # 775
tokenlite_app/storage/app/kyc-files/    # 775
tokenlite_app/storage/app/public/       # 775
tokenlite_app/bootstrap/cache/           # 775
You must set these folders framework, logs, kyc-files, cache permission to 775 as above. Sometimes base on server permission 775 may not work, then you have to set 777

Before start the installation process please fulfill the server requirements as bellow.

- PHP >= 7.3 (support upto 7.4)
- OpenSSL PHP Extension
- PDO PHP Extension
- Mbstring PHP Extension
- Tokenizer PHP Extension
- XML PHP Extension
- Ctype PHP Extension
- JSON PHP Extension
- BCMath PHP Extension
- FileInfo PHP Extension

Manual Installation Process
Step One: Configure .ENV File
Please go to tokenlite_app folder and edit the .env file. On this file please use bellow code and update accordingly to your information and save the file.

Please you must change these value -
APP_NAME, APP_URL, DB_HOST, DB_DATABASE, DB_USERNAME, DB_PASSWORD

APP_NAME='YOUR_APP_NAME_HERE'
APP_VERSION='1.0.0'
APP_ENV=production
APP_KEY=base64:bMzV/BygkgeonjHpn5c7NkwcAi8ckl+tBIEfNfOqgmw=
APP_DEBUG=false
APP_LOG_LEVEL=debug
APP_URL=http://yourdomainname.com

FORCE_HTTPS=false
DB_CONNECTION=mysql
DB_HOST=127.0.0.1
DB_PORT=3306
DB_DATABASE=your_db_name
DB_USERNAME=your_db_user_name
DB_PASSWORD=your_db_password

BROADCAST_DRIVER=log
CACHE_DRIVER=file
SESSION_DRIVER=file
QUEUE_DRIVER=sync

REDIS_HOST=127.0.0.1
REDIS_PASSWORD=null
REDIS_PORT=6379

MAIL_DRIVER=smtp
MAIL_HOST=smtp.mailtrap.io
MAIL_PORT=2525
MAIL_USERNAME=null
MAIL_PASSWORD=null
MAIL_ENCRYPTION=null

PUSHER_APP_ID=
PUSHER_APP_KEY=
PUSHER_APP_SECRET=
Step Two: Installed File placement
Please copy the installed file (found under manual-install-files folder) and placed into tokenlite_app/storage folder.

Step Three: Import Dummy SQL File
Please import the sql file dummy_app.sql into your database.
File found under manual-install-files folder.

Final Step
Once above step are complete please go to your website url. https://your-domain.com/ & register first your Super Admin account. Then login to your account and configure the Website settings, Email settings, Payment settings and ICO Stages etc.

Note: First registered user will be always super-admin privilege.


