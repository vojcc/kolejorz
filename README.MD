<p align="center">
    <img src="https://user-images.githubusercontent.com/92044526/218345559-5b423bc6-4131-46c5-825c-297169ebcea0.gif" width="250" height="350"/>
    <img src="https://user-images.githubusercontent.com/92044526/218345563-54ae14ad-ef80-401b-aa91-721a7e74dc17.gif" width="465" height="350"/>
</p>

<p align="center">
    <img src="https://user-images.githubusercontent.com/92044526/218345566-909bb725-2e5a-4aa6-8e73-1c5490ffb142.gif" width="488" height="311"/>
    <img src="https://user-images.githubusercontent.com/92044526/218345569-66da71af-f133-48f8-875e-25a357a11ea4.gif" width="488" height="311"/>
</p>



# Installation

## 1. Clone repository
`git clone https://github.com/grinmilksoftware/kolejorz`

## 2. Move into directory you've created
`cd kolejorz`

## 3. Install dependencies
`docker run --rm -v $(pwd):/app composer install`
### You can change the ownership of directory to non root user
`sudo chown -R $USER:$USER kolejorz`

## 4. Create .env file based on .env.example
`cp .env.example .env`

## 5. Run containers
`./vendor/bin/sail up`

## 6. Generate key
`./vendor/bin/sail artisan key:generate`

## 7. Install dependencies
`npm install`

## TroubleShooting
in case of runnig this program on linuxbase system, you may encounter an error about Permission denied. Simple fix to that may be add  <br>
`WWWGROUP=1000` <br>
`WWWUSER=1000` <br>
to .env file
