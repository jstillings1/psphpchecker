# psphpchecker
This is a mod off the prestashop php checker that removes the session use for broken server troubleshooting
My current production settings are 
PHP Configuration
# 	            Required 	      Recommended 	      Current
allow_url_fopen 	  Yes 	        Yes 	              Yes
expose_php 	        No 	          No                  Yes # left on so clients can call and say more then its broke
file_uploads      	Yes 	        Yes 	              Yes
register_argc_argv 	No 	          No 	                No
short_open_tag 	    No 	          No 	                No
max_input_vars 	    1000 	        5000 	              30000 #With product combinations I might even have to go higher
memory_limit 	      64M 	        256M 	              1024M # the prodcut combo generation button EATS ram 1024 is lowest can use
post_max_size 	    16M 	        128M              	128M
upload_max_filesize 4M 	          128M 	              128M
set_time_limit 	    Yes 	        Yes 	              Yes
