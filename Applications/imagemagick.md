# Image magick

[link](https://askubuntu.com/questions/1127260/imagemagick-convert-not-allowed)

ImageMagick has some security policies disabling some rights for security reasons. See why at the bottom of this answer.
You will have to edit a config file to re-enble the action you need.

Open **/etc/ImageMagick-6/policy.xml** with your favorite text editor,
find the line 
```
<policy domain="coder" rights="none" pattern="PDF" />
```
and replace **"none"** by **"read|write"**

```

# Open the file 
sudo nvim /etc/ImageMagick-6/policy.xml

# find and edit the line
<policy domain="coder" rights="none" pattern="PDF" />
# to :
<policy domain="coder" rights="read|write" pattern="PDF" />
```
