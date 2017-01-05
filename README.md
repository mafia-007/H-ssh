# H-ssh

### INSTALL
```
git clone http://github.com/mafia-007/H-ssh

sudo apt-get install python-requests python-lxml 
OR
pip install -r requirements.txt
```

### HELP
```
usage: 
 ██████╗ ██╗████████╗███╗   ███╗██╗███╗   ██╗███████╗██████╗ 
██╔════╝ ██║╚══██╔══╝████╗ ████║██║████╗  ██║██╔════╝██╔══██╗
██║  ███╗██║   ██║   ██╔████╔██║██║██╔██╗ ██║█████╗  ██████╔╝
██║   ██║██║   ██║   ██║╚██╔╝██║██║██║╚██╗██║██╔══╝  ██╔══██╗
╚██████╔╝██║   ██║   ██║ ╚═╝ ██║██║██║ ╚████║███████╗██║  ██║
 ╚═════╝ ╚═╝   ╚═╝   ╚═╝     ╚═╝╚═╝╚═╝  ╚═══╝╚══════╝╚═╝  ╚═╝ v1.1
 Automatic search for GitHub.                                                            

 + Autor: Danilo Vaz a.k.a. UNK
 + Blog: http://unk-br.blogspot.com
 + Github: http://github.com/mafia-007/H-ssh
 + Gr33tz: l33t0s, RTFM

 +[WARNING]------------------------------------------+
 | THIS TOOL IS THE PENALTY FOR EDUCATIONAL USE,     |
 | THE AUTHOR IS NOT RESPONSIBLE FOR ANY DAMAGE TO   |
 | THE TOOL THAT USE.                                |
 +---------------------------------------------------+


       [-h] [-q 'filename:shadown path:etc']
       [-m wordpress] [-o result.txt]

optional arguments:
  -h, --help            show this help message and exit
  -q 'filename:shadown path:etc', --query 'filename:shadown path:etc'
                        Specify search term
  -m wordpress, --module wordpress
                        Specify the search module
  -o result.txt, --output result.txt
                        Specify the output file where it will be
                        saved
```

### EXAMPLE
Searching for wordpress configuration files with passwords:
```
$:> python git_miner.py -q 'filename:wp-config extension:php FTP_HOST in:file ' -m wordpress -o result.txt
```
![Screenshot](https://2.bp.blogspot.com/-GbpzROiEynQ/VtLytfMqQiI/AAAAAAAAbnk/5hDphP4Mbf4/s1600/wordpressEX.png)

Looking for brasilian government files containing passwords:
```
$:> python git_miner.py --query 'extension:php "root" in:file AND "gov.br" in:file' -m senhas
```

Looking for shadow files on the etc paste:
```
$:> python git_miner.py --query 'filename:shadow path:etc' -m root
```

Searching for joomla configuration files with passwords:
```
$:> python git_miner.py --query 'filename:configuration extension:php "public password" in:file' -m joomla
```
![Screenshot](https://3.bp.blogspot.com/-1AsNmFKfsoA/VtLyvJFy2WI/AAAAAAAAbno/C7xTbxtzOo8/s1600/joomlaEX.png)

