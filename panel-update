echo -e "\e[1;31m Your Pterodactyl Update Is Now Starting! \e[0m"
sleep 3
cd /var/www/pterodactyl
sleep 1
php artisan down
sleep 1
curl -L https://github.com/pterodactyl/panel/releases/latest/download/panel.tar.gz | tar -xzv
sleep 1
chmod -R 755 storage/* bootstrap/cache
sleep 1
composer install --no-dev --optimize-autoloader
sleep 1
php artisan view:clear
sleep 1
php artisan config:clear
sleep 1
php artisan migrate --seed --force
sleep 1
chown -R www-data:www-data /var/www/pterodactyl/*
sleep 1
php artisan queue:restart
sleep 1
php artisan up
sleep 1
clear
sleep 1
echo -e "\e[1;31m Your Pterodactyl Update Has Now Been Completed | Made By PrestonJude :D \e[0m"
sleep 10
