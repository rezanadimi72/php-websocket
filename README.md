
# Installation
1. Clone the repository from Github using — “git clone https://github.com/rezanadimi72/php-websocket.git”
2. Place the cloned folder to your local server.
3. Now open cmd in this in the cloned directory and run — “composer install”
4. Create new database “realtimechat“ then import table ”socket_id” for the sql given below.
5. Change database configuration according to your username and password in ”src/App/Chat.php” (line 24 to 29).
4. Then change directory to bin folder by — “cd bin”
5. Stat-server by — “php -q chat-server.php”
6. Now hit public folder of the project by your browser — “localhost/path_to_your_folder/public”
7. Done!

# Database table
CREATE TABLE `socket_id` (
  `id` int(11) NOT NULL AUTO_INCREMENT,
  `user` varchar(255) DEFAULT NULL,
  `socket_id` int(11) DEFAULT NULL,
  PRIMARY KEY (`id`)
)
