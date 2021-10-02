# Minecraft server status page
A simple page to see if your minecraft server is online with some basic stats like the version and amount of players online.

## Requirements
- A webserver with php >= 7
- [Composer](https://getcomposer.org/)

## Setup
1. Clone this repository on your webserver.
2. Duplicate the `.env.example` file to `.env` and update this file with the settings that apply to you. (do this for every server you have into a new .env2, .env3, etc file)
  2.1. add SERVER_HOST which is the actual IP or hostname of your server without port, NAME which is a nickname for the server, PORT which is the serverport
4. From within the project directory run `composer install` to download and install the dependencies.
5. Point your webserver to the `public` dir of this project and the Minecraft server status page is up and running.
6. You will have to copy/paste the server block between "-----SERVER START-----" and "-----SERVER STOP-----" for each server you want to add.
7. make sure the sections for header and footer are added to the first and last server block to maintain the desired layout.

## Screenshot
![dummy screenshot](https://raw.githubusercontent.com/kenshin133/MinecraftStatusPage/master/photo_2021-10-02_15-34-14.jpg)

TODO:

simplify the use of the .env files to allow use of 1 file for multiple server info and limit manual changes.
simplify the addition of servers, preferably it should spawn more server blocks as more servers are added to whatever config file or env file I end up using.
Move header block out of the first server block
move footer out of last server block
