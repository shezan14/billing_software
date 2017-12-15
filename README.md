# Billing Software

This is a billing software for any store.
Its will calculate product price tax discounts &amp; generate a receipt customer. No database need . 

* mobile responsive
* no need any database for full process.
* if you want can connect database.
* You can print receipt & customize size.


For use :

composer require arman/billing_software


in confiq/app.php :

	'providers' => [
	
		arman\billing_software\billingSoftwareProvider::class,

	]
	
	
in composer.json :

replace this

'composer.json' => [

	"autoload": {
		"classmap": [
		    "database"
		],
		"psr-4": {
		    "App\\": "app/",
		    "arman\\billing_software\\": "vendor/arman/billing_software/src"
		}
	    }
	    
]	

in cmd :

composer dump-autoload -o


in route :

http://localhost/auth/public/bill
