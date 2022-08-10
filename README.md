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
