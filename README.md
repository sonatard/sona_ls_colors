sona_ls_colors
==============

LS_COLORS setting file for many files and many programming language

# Usage 
This file goes in the /etc directory, and must be world readable.
You can copy this file to .dir_colors in your $HOME directory to override
the system defaults.

```sh
git clone https://github.com/sona-tar/sona_ls_colors.git
cd sona_ls_colors
cp .dir_colors ~/
dircolors -b ~/.dir_colors
```

vi ~/.zshenv
```sh
[ -z $LS_COLORS ] && eval `dircolors -b ~/.dir_colors`
```

zsh completion color same as GNU ls color
vi ~/.zshrc
```sh
zstyle ':completion:*' list-colors ${(s.:.)LS_COLORS}
```

# Screenshot
## file type
![ls_colors file_type](http://cdn-ak.f.st-hatena.com/images/fotolife/s/sona-zip/20130622/20130622182607_original.png)

## C

![ls_colors c](http://cdn-ak.f.st-hatena.com/images/fotolife/s/sona-zip/20130622/20130622213213.png)

## web
![ls_colors web](http://cdn-ak.f.st-hatena.com/images/fotolife/s/sona-zip/20130622/20130622213236.png)



# extension examples
## execute
exe,com,app,bin

## documet
txt,md,tex,pod,csv,json

## source file
asm,c,cpp,cxx,java,.ll.scala,ml,sql,vhd,yacc,sh,pl,rb,py,bat,vbs,lisp,scm,vim,el,cgi,jsp,js

## header
h,hpp,inc

## diff
patch,diff

## markup
html,xml,sgml,xaml,yaml,rdf

## stylesheet
css,xsl,xslt

## Library
so,sl,lib,a,dll

## object , byte code
o,obj,cmx,class,pyc,pyo,elc,

## config
config,conf,cfg,shrc,init,inf,reg,recipe,repo,mf,mk,allow,deny,htaccess,htpasswd

## Linux System
loc,pid,mo

## VCS
cvs,svn,git

## binary data
man,map,ram,rom,db,pcap

## image
bmp,jpg,gif,png,pps,ps,svg,tif

## raw image
raw,ARW(sony),CRW,CR2(canon),DNG(PENTAX),KDC(Kodak),ERF(ePSON)...

## image information
exif

## audio
aac,au,flac,mid,mp3,mpa,mpg,ogg,wav

## movie
avi,flv,mp4,mpg,ogm,rm,wmv,ts

## font
otf,ttc,ttf

## binary doc
doc,docx,rtf,dot,dtx,xls,xlsx,xlt,xltx,ppt,pptx....

## multimedia binary
fla,psd,xcf,xdw

## archives
7z,bin,bz,bz2,cab,deb,dmg,gem,gz,iso,img,jar,lzh,msi,rar,rpm,tar,tbz,tbz2,tgz,war,xpi,xz,zip

## unimportant files
*~,*#,bak,BAK,old,OLD,orig,ORIG,swp

## security
pub,crt,key,rsa,sig

