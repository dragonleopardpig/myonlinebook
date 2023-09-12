
# Table of Contents

1.  [Note](#orge18a1b1)
2.  [Planned Software Development](#org52ead0a)
    1.  [Regular Expression](#orgbe34305)
    2.  [Database](#org8a6fbf7)
    3.  [Image Analysis](#org1061f6d)
    4.  [Design of Experiment](#org3fdbd67)
    5.  [Jupyter BOOK](#org75287c5)
    6.  [Git](#org02f984e)
3.  [Command](#orgfe2fe97)
4.  [Others](#org240d5d2)
    1.  [R Babel](#org7a2ec8c)
        1.  [produce a file, by using :results output](#org3859d97)
        2.  [produce a file, by printing object](#orgdc18b28)
        3.  [produce a file, by evaluating in :session](#orgb4bb9e7)
    2.  [Jupyter](#org94d2899)
5.  [Encryption](#org76e5530):crypt:


<a id="orge18a1b1"></a>

# Note


<a id="org52ead0a"></a>

# Planned Software Development


<a id="orgbe34305"></a>

## TODO Regular Expression

-   Sed and Awk


<a id="org8a6fbf7"></a>

## TODO Database

-   Postgresql
-   Sqlite3


<a id="org1061f6d"></a>

## TODO Image Analysis

-   scikit-image


<a id="org3fdbd67"></a>

## TODO Design of Experiment

-   R


<a id="org75287c5"></a>

## Jupyter BOOK


<a id="org02f984e"></a>

## Git

-   


<a id="orgfe2fe97"></a>

# Command

-   cryfs -c cryfs.config basedir mountdir
-   cryfs-unmount mountdir
-   restic -r *home/plchu/pCloudDrive* &#x2013;verbose backup *home/plchu/mountdir* -p *home/plchu/mountdir*.restic
-   0 \* \* \* \* root restic -r *home/plchu/pCloudDrive/mountdir* &#x2013;verbose backup *home/plchu/mountdir* -p *home/plchu/mountdir*.restic
-   restic -r *home/plchu/pCloudDrive/mountdir* -p *home/plchu/mountdir*.restic snapshots
-   sudo systemctl status cron.service


<a id="org240d5d2"></a>

# Others


<a id="org7a2ec8c"></a>

## R Babel


<a id="org3859d97"></a>

### produce a file, by using :results output

    library(lattice)
    xyplot(1:10 ~ 1:10)


<a id="orgdc18b28"></a>

### produce a file, by printing object

    library(lattice)
    print(xyplot(1:10 ~ 1:10))


<a id="orgb4bb9e7"></a>

### produce a file, by evaluating in :session

    library(lattice)
    xyplot(1:10 ~ 1:10)


<a id="org94d2899"></a>

## Jupyter

-   C-c ' to edit first before run by C-c C-c, otherwise it hangs.

    from sympy import *
    from IPython.display import display
    init_printing()
    x, y, z = symbols('x y z')
    
    display(Integral(sqrt(1 / x), x))

![img](./.ob-jupyter/723f9db74b6fb21a7972623b0b92881f90cbb006.png)


<a id="org76e5530"></a>

# Encryption     :crypt:

&#x2013;&#x2014;BEGIN PGP MESSAGE&#x2013;&#x2014;

jA0ECQMCKp4OQ1U9VV3/0mABCTF60aKFPtbJIpbfjkRsSUDc8vLaaEpmICSTd8Hg
F/djqA4WScRtng9SAKDoPgSsN4AgpKQZ2vOqLwhyNDw3rkGkbQN/EZLPeu8CC7So
aS9ejnrvrQ1UWNdSNyDOSc0=
=Icfd
&#x2013;&#x2014;END PGP MESSAGE&#x2013;&#x2014;

