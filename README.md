# covid19_spreading


To work geopandas properly use install guide from main site: https://geopandas.org/install.html

After receiving images in png format, you can make a video, using ffmpeg util:

<code>
sudo add-apt-repository ppa:jonathonf/ffmpeg-4
</code>
<br>
<br>
This PPA contains packages for Ubuntu 18.04 (Bionic) and 16.04 LTS (Xenial) only.
<br>
<br>
<code>
sudo apt-get update
</code>
<br>
<code>
sudo apt-get install ffmpeg
</code>
<br><br>
<code>ffmpeg -framerate 30 -pattern_type glob -i '*.png' -c:v libx264 -pix_fmt yuv420p out.mp4</code><br><br>
Example for 8.4.20:
