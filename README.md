# certtools
Linux scripts for simpler SSL administration on linux servers in conjunction with StartSSL.
StartSSL is not mandatory and the scripts can be changed easy.

## Installation

Clone the repository and create the certs-subdirectory. 

    git clone https://github.com/hberndt/certtools.git
	mkdir certs
	
	
## Usage

Generate a new certificate by editing newcert.cnf and start 
    
    newcert <domain>.

Retrieve a certificate of a site by calling 
    
    retrieve <URL> <filename>.

Use show to get all certificates in clear text from ./certs directory.

You can show one certificate using 
    
    show <filename>.

If you need a JAVA keystore you can install a certificate using
    
    ksimport alias certificate [keystore]

Updating a JAVA keystore is done by
    
    ksupdate alias certificate [keystore]

ksimport/ksupdate load the certificate from ./certs. ./certs is the private 
certification store.