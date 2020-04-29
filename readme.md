***The included source code, service and information is provided as is, and OmniUpdate makes no promises or guarantees about its use or misuse. The source code provided is recommended for advanced users and may not be compatible with all implementations of OU Campus.***

# Ruby Migration

## Required Gem
	- Please install the OS Gem
	- `gem install OS` or `sudo gem install OS`

## Global (\_global)
	- Contains the global methods and classes for all migrations.
	- ***This is always needed for all migrations.***

## Skeletons

Choose the appropriate package depending on the type of migration you expect to perform as follows:

1. `migrate_shell_csv.rb`
	- Used to create a shell site, given a migration map (CSV format). 
2. `migrate_from_source.rb`
	- Used to perform a 1-to-1 migration from a set of source files. 
3. `migrate_from_csv.rb`
	- Used to perform a migration from a set of source files, rearchitecting the files during migration using a migration map (CSV format). 

Once you have chosen the appropriate skeleton package, you will need to adjust the configuration with the proper variables, set your templates to match the OU Campus PCF output required for your implementation, and target your content using XPath. The script will output a file package that can then be zipped and uploaded into OU Campus for immediate use. 