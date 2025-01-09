# grep overview

Use it to search for a particular keyword.
Ex: grep "error" /var/log/container/file.log

### useful flags:
    - -c for the count
    - -v for excluding that keyword
    - -i for ignoring the case

We can obviously pass grep via pipe

# sed overview

sed =  stream editor
most commonly used for find and replace stuff within files
Example:
    sed 's/bash/zsh/g' file.txt
        -> s =  substitute
        -> bash = original
        -> zsh = target
        -> g = globally
        -> file.txt = the file in which this needs to be done
**The above command will substitute 'bash' with 'zsh' globally (all instances) in file.txt file. **

-> *But this doesn't modify the original flag. To modify the original flag, we need to use ''-i' flag. *
-> *Instead of 'g' if we use '1', then it'll replace the original with target wherever it is occuring for the first time in each row/line *

# awk overview

Used in Linux mainly for text processing

#### Example:
dummy.txt :-
------------

Name        LastName        Email
abc         zz              abc@gmail.com
pqr         yy              pqr@gmail.com

EOF

-> awk '{print $1}'     => prints Name column
-> awk '{print $1,$2}'  => prints Name and LastName column (space seperated)

dummy.txt :-
------------

Name:LastName:Email
abc:zz:abc@gmail.com
pqr:yy:pqr@gmail.com

EOF

Now everything is seperated by ':' instead of space like before

-> awk -F: '{print $1,$2}'  => prints Name and LastName column (space seperated)
    ** We are specifing ':' as delimiter using '-F' flag **

