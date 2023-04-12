almalinux

```
dnf install epel-release -y
dnf config-manager --set-enabled crb
dnf install --nogpgcheck https://mirrors.rpmfusion.org/free/el/rpmfusion-free-release-$(rpm -E %rhel).noarch.rpm -y
dnf install --nogpgcheck https://mirrors.rpmfusion.org/nonfree/el/rpmfusion-nonfree-release-$(rpm -E %rhel).noarch.rpm -y
dnf install ffmpeg ffmpeg-devel -y
ffmpeg -version
```
```
dnf install wget -y
wget https://github.com/yt-dlp/yt-dlp/releases/download/2023.03.04/yt-dlp_linux
mv yt-dlp_linux yt-dlp
chmod +x yt-dlp
```
查看分辨率
```
./yt-dlp -F https://www.youtube.com/watch?v=NpEd2S6iQZI
```
下载对应分辨率
```
./yt-dlp -f313 https://www.youtube.com/watch?v=NpEd2S6iQZI
```
