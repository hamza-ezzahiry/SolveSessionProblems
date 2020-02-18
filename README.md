# SolveSessionProblems

[![All Contributors](https://img.shields.io/badge/all_contributors-1-red.svg?style=flat-square)](#contributors-)


<p align="center">
  <a href="http://1337.ma/"Solve Session Problems">
    <img alt="Gatsby" src="https://i.imgur.com/jm1e5Hk.jpg" width="300" />
  </a>
</p>
<h1 align="center">
  Solution to each problem
</h1>

### About

This repo for 1337 students where they can find solutions of every session problem 



# SolveSessionProblems

<img src="https://images.yourstory.com/cs/wordpress/2018/02/image_2.png" width="400" height="200">



**Problem List:**

- [x] Problem 1 : Full disk
- [x] Problem 2 : ctkahp quit unexpectedly
- [x] Problem 3 : iscsi-target problem
- [x] Problem 4 : install brew 
- [x] Problem 5 : No more .DS_Store
- [x] Problem 6 : Norminete Time-out
- [x] Problem 7 : Unavailable



## Solutions : 


### Problem 1 : Full disk

easy, use this tool **[Cclean](https://github.com/su-omb/Cleaner_42)** developed by the student : Omar Bouykourne.

### Problem 2 : ctkahp quit unexpectedly

You have to remake the symbolic links to goinfre directories and also clean the Chrome cache.

### Problem 3 : iscsi-target problem 

New service is deployed by 1337 Staff **[iscsi-tools](https://iscsi-tools.1337.ma)** , so you could by yourself fix iscsi-target problems, first you have to login in intra (using your mobile phone or your peer computer) and click on fix iscsi. (easy-peasy 😁)

### Problem 4 : install brew 

script 1:
```sh

#!/usr/sh 
rm -rfv $HOME/.brew && git clone --progress --verbose --depth=1 https://github.com/Homebrew/brew $HOME/.brew && echo 'export PATH=$HOME/.brew/bin:$PATH' >> $HOME/.zshrc && source $HOME/.zshrc && brew update -v 
```

script 2:

```sh

rm -rf $HOME/.brew && git clone --depth=1 https://github.com/Homebrew/brew $HOME/.brew && export PATH=$HOME/.brew/bin:$PATH && brew update && echo "export PATH=$HOME/.brew/bin:$PATH" >> ~/.zshrc
```

### Problem 5 : No more .DS_Store

script :
```sh
  find ~Desktop -name .DS_Store -depth -exec rm {} \; 
```
**P.S :** Add it as an alias  

### Problem 6 : Norminete Time-out

<img src="https://thijsdejong.gallerycdn.vsassets.io/extensions/thijsdejong/codam-norminette/19.10.1/1572359486186/Microsoft.VisualStudio.Services.Icons.Default" width="100" height="100">

Use this tool **[codam-norminette-plus](https://github.com/thijsdejong/codam-norminette-plus)** and you can also use this extension on vs code **[Codam Norminette](https://marketplace.visualstudio.com/items?itemName=thijsdejong.codam-norminette)**


### Problem 7 : Unavailable

<img src="https://i.imgur.com/c4uy3cM.png" width="400" height="100">

To solve this problem follow these steps : 

**1. open iTerm** 


**2. execute the following command until you find this result "kdestroy: krb5_cc_destroy: No credentials cache file found"** 

```sh
 $ kdestroy
```

**3. execute and fill-in it with your infos** 
```sh
 $ kinit
```

**4. Go to SETTINGS -> Security.**

click here : [link](https://profile.intra.42.fr/securities)

And click on :

<img src="https://i.imgur.com/eer6D71.png" width="300" height="100">

**5. Finally, log out from your session and re-login**
