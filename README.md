# Google Integrated System Conky
This is my Arch linux conky configuration with conky, lua, Google Calendar and Google Keep

<a href='https://ko-fi.com/B0B2TZMH' target='_blank'><img height='36' style='border:0px;height:36px;' src='https://az743702.vo.msecnd.net/cdn/kofi1.png?v=2' border='0' alt='Buy Me a Coffee at ko-fi.com' /></a>

<img src="https://i.postimg.cc/CMFRTkqb/gisc-1.png?dl=1" />

# Supports

- Google Calendar Integration
- Google Keep Integration
- RSS feed integration
- Basic system information table(CPU,RAM,HDD/SSD,Date/Time ...)

# Installation
- <b>Ubuntu & Derivatives</b>

```
sudo apt install conky-all python3-pip python-pip git; sudo pip3 install beautifulsoup4 requests lxml ; sudo pip install gcalcli ; git clone https://github.com/mustafaozhan/GoogleIntegratedSystemConky ; cd GoogleIntegratedSystemConky/ ; chmod +x install.sh && sh ; install.sh
```

- <b>Arch Linux & Derivatives</b>

```
sudo pacman -S python-pip python2-pip git; git clone https://aur.archlinux.org/package-query.git ; cd package-query/ ; makepkg -si ; cd .. ; git clone https://aur.archlinux.org/yaourt.git ; cd yaourt ; makepkg -si ; cd .. ; rm -rf yaourt/ package-query ; yaourt -S conky-lua ; sudo pip3 install beautifulsoup4 requests lxml ; sudo pip2.7 install gcalcli ; git clone https://github.com/mustafaozhan/GoogleIntegratedSystemConky ; cd GoogleIntegratedSystemConky/ ; chmod +x install.sh && sh install.sh
```

- Go to the ~/.config/GoogleIntegratedSystemConky/background/ and choose a wallpaper and add your profile picture in the circle (You can use gimp as a editor and for good looking you can make it grayscale)

- In ~/.config/GoogleIntegratedSystemConky/config.xml put your google mail address and password for notes

- start with
```
sh ~/.config/GoogleIntegratedSystemConky/gisc.sh start
```

- In first time a windows with your default browser will be openned and it will ask for your gmail permission for calendar. After that if it will print any error on the desktop kill conky with 
```killall conky``` than start it back with ```sh ~/.config/GoogleIntegratedSystemConky/gisc.sh start```

# Configuration
Configuration based on 1600*900. Change it acording to your screen resolution.

- Xfce panel size is 44
- plank Icon size is 44
- Xfce panel color is same as background
- You have to have your notes titled To-do in your Google Keep. (To change it ~/.config/GoogleIntegratedSystemConky/config.xml)

If you will have so much notes in your Google Keep or events in your Google Calendar panel will not cut your rows by this configurations.

# Thanks to
<a href="https://github.com/kunesj/conkyKeep">conkyKeep</a> for Google Keep integration, <a href="https://github.com/insanum/gcalcli">gcalcli</a> for Google calendar integration. And lastly apperance highly customized from  <a href="https://blog.icanbeacoder.com/inifinity-dark-conky-theme-v2/">inifinity-dark-conky-theme-v2</a>
