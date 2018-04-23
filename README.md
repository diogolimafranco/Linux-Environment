# Linux Environment
My environment linux 16.04

sudo apt-get update && \
sudo apt-get -y upgrade && \

# Install all dependencies
sudo apt-get -y install \
apache2 \
git \
php7.0 \
php7.0-curl \
php7.0-gd \
php-xdebug \
libapache2-mod-php7.0 \
ruby-full \
nodejs \
npm \
libpng12-0 \
libpng12-dev \
filezilla \
kazam \
vlc \
ruby-sass \
python-pip && \

# Install Image Compressor Guetzli by Google
git clone https://github.com/google/guetzli.git
cd guetzli
make
sudo cp bin/Release/guetzli  /usr/bin/
| guetzli --quality 85 image.jpg image-out.jpg

# Install Skype
https://www.skype.com/pt-br/get-skype/

# Install Visual Studio Code
https://code.visualstudio.com

# Install Sublime Text 3
https://www.sublimetext.com/

# Install Google Chrome
https://www.google.pt/intl/pt-PT/chrome/

# Configure Apache
| Alter root folder to my workspace in Desktop

ln -s /home/diogo/Área\ de\ Trabalho/ /home/diogo/Desktop

mkdir /home/diogo/Desktop/projects

sudo chmod 777 -R /home/diogo/Desktop/projects

sudo subl /etc/apache2/apache2.conf

sudo subl /etc/apache2/sites-available/000-default.conf || sudo vim /etc/apache2/sites-available/default.conf

service apache2 restart

# Sublime Text Config
{
	"always_show_minimap_viewport": true,
	"bold_folder_labels": true,
	"color_scheme": "Packages/Dracula Color Scheme/Dracula.tmTheme",
	"draw_minimap_border": true,
	"font_size": 14,
	"highlight_line": true,
	"highlight_modified_tabs": true,
	"ignored_packages":
	[
		"Vintage"
	],
	"line_padding_bottom": 10,
	"line_padding_top": 10,
    "tab_size": 2,
	"theme": "Material-Theme-Palenight.sublime-theme",
	"translate_tabs_to_spaces": true,
	"word_wrap": true
}
