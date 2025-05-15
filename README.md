# Node-run-build-React-Project
For building React project

1. กำหนด path ของ folder เช่น /devop/oem/pre-assembly
2. <BrowserRouter basename="/devop/oem/pre-assembly">
3. เก็บ api.php ไว้ใน folder -> /devop/oem/pre-assembly/api
Ex. Request [HTTP Method] /devop/oem/pre-assembly/api/api.php
4. npm run build จะได้ dist folder -> assets/, index.html
และแก้ path "/assets... เป็น "./assets...

5. สร้างไฟล์ .htaccess ไฟล์
Script:
    Options -MultiViews
    RewriteEngine On
    RewriteCond %{REQUEST_FILENAME} !-f
    RewriteRule ^ index.html [QSA,L]


<link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/6.1.1/css/all.min.css" integrity="sha512-KfkfwYDsLkIlwQp6LFnl8zNdLGxu9YAA1QvwINks4PhcElQSvqcyVLLD9aMhXd13uQjoXtEKNosOWaZqXgel0g==" crossorigin="anonymous" referrerpolicy="no-referrer" />