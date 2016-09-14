## Basic step
## Self Experience
### From remote repository
* Create Repository in github and get .git like https://github.com/yaodongsh/src.git
* In local, use `git clone https://github.com/yaodongsh/src.gi`t
* Add file into this directory, use `git add`, `git commit`
* `git push -u origin master` (or just `git push`)
### Basic step in local
#### start from None
* Go to one directory:

	    md git
	    cd  git
	    git init

* add some config  

	    git config --global user.name 'xx'
	    git config --global user.email 'xx@xx.com'

* add file (for a new file, like p4 add, for an existing file, like p4 edit)  
    	
 		git add my_file

* commit
  
	    git commit -m "xxxxxxx"

#### for an existing file
* `git add` (like p4 edit)
* do some change
* `git commit -a`  (need understand why -m not work??)
* use git log to track edit history  
`git log -p`

