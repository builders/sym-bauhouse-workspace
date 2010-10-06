# Bauhouse - A Symphony Ensemble Workspace

- Author: Stephen Bau
- Version: 0.2
- Date: 5 October 2010
- Github Repository: <http://github.com/builders/sym-bauhouse-workspace>
- Download: <http://symphony-cms.com/download/ensembles/view/41702/>
- Forum Discussion: <http://symphony-cms.com/discuss/thread/41703/>

## Release Notes

#### [Version 0.2](http://github.com/builders/sym-bauhouse-workspace/commits/0.2)

- Date: 5 Oct 2010
- Update to Symphony 2.1.1

#### [Version 0.1](http://github.com/builders/sym-bauhouse-workspace/commits/0.1)

- Date: 22 March 2010
- Initial Release
- Symphony 2.0.7

## Overview

### My old portfolio site

It's about time I updated my site. It might need a design refresh, but I still like the old site. With the freelance business a thing of the past, it might be nice to share the old site design, but brought back to life, now updated to the latest version of Symphony 2.1.1.

Visit the old site at <http://bauhouse.ca/>

## Installation

### Note: This is a work in progress

It is best to install this ensemble with Git, but you can also install this ensemble by downloading a copy of Symphony 2.1.1 and each of the required extensions and this workspace. 

### Installing with Git the easy way

1. Clone the Bauhouse Ensemble repository and rename the directory (if you like):

		git clone git://github.com/builders/sym-bauhouse-ensemble.git bauhouse

2. Change directory:

		cd bauhouse

3. Update all submodules, which will include all extensions and the workspace directory:

		git submodule update --init

		or, if that doesn't work, issue the commands separately:

		git submodule init
		git submodule update

4. Install the ensemble as you would normally install Symphony by pointing your 
web browser at <http://yourwebsite.com/install.php> and provide details for
establishing a database connection and about your server environment.
		
### Installing with Git the long way

1. Clone a copy of Symphony 2.1.1. into a directory called `bauhouse`:

		git clone git://github.com/symphonycms/symphony-2.git bauhouse

2. Change directory:

		cd bauhouse
		
3. Initialize the submodules for the default extensions:

		git submodule init
		git submodule update

4. Add the required extensions as submodules:

		git submodule add git://github.com/carsten/collapse_sectionfields.git extensions/collapse_sectionfields
		git submodule add git://github.com/pointybeard/content_type_mappings.git extensions/content_type_mappings
		git submodule add git://github.com/czheng/enhancedtaglist.git extensions/enhancedtaglist
		git submodule add git://github.com/bauhouse/export_install_file.git extensions/export_install_file
		git submodule add git://github.com/carsten/globalparamloader.git extensions/globalparamloader
		git submodule add git://github.com/rowan-lewis/globalresourceloader.git extensions/globalresourceloader
		git submodule add git://github.com/ahwayakchih/markitup.git extensions/markitup
		git submodule add git://github.com/pointybeard/numberfield.git extensions/numberfield
		git submodule add git://github.com/nickdunn/order_entries.git extensions/order_entries
		git submodule add git://github.com/pointybeard/pagesfield.git extensions/pagesfield
		git submodule add git://github.com/nickdunn/publishfiltering.git extensions/publishfiltering
		git submodule add git://github.com/rowan-lewis/logsdevkit.git extensions/logsdevkit
		git submodule add git://github.com/nickdunn/entity_diagram.git extensions/entity_diagram
		git submodule add git://github.com/czheng/referencelink.git extensions/referencelink
		git submodule add git://github.com/rowan-lewis/reflectionfield.git extensions/reflectionfield
		git submodule add git://github.com/nickdunn/section_schemas.git extensions/section_schemas

5. Clone the Symphony workspace for Bauhouse to a directory called `workspace`:

		cd ..
		git clone git://github.com/builders/sym-bauhouse-workspace.git workspace

6. Set permissions to allow Symphony to write files to the server:

		chmod 777 symphony .
		chmod -R 777 workspace

7. Be sure to have an empty database ready for Symphony (or use a different table prefix). Navigate to the root of the install and provide your preferences, server configuration details and primary user information and click the "Install" button to install Symphony 2 and the Bauhouse ensemble.

8. Secure the site by changing permissions for the root and symphony directories.

		chmod 755 symphony .

9. Enjoy seeing the world in black, white, grey and a touch of red!