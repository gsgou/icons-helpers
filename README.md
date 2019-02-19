# icon-tools

Bash script to ***process icons*** for mobile-development use cases.

Uses imagemagick (`convert`) (`mogrify`) to manipulate the image input.
  
## Example Runs

```
$ icon-tools.sh colorize $FILE "rgb(255,0,0)"
$ icon-tools.sh colorize $FILE "#FF0000FF"
$ icon-tools.sh createicons $FILE 48
$ icon-tools.sh dominantcolor $FILE
$ icon-tools.sh resize $FILE 24
$ icon-tools.sh square $FILE transparent
$ icon-tools.sh trim $FILE
```
## Dependencies

The script uses `basename`,`dirname`,`grep`,`head`,`mkdir`,`mv`,`rm`,`sed`,`sort`,`convert` and `mogrify`.

##### apt-get
```
sudo apt-get install imagemagick
```
##### yum
```
sudo yum install imagemagick
```
##### homebrew MacOS
```
brew install imagemagick --build-from-source
```