## Installation ##

You can use two methods to install activationbymail module:
  1. Automatic
  1. Manual

Automatic installation is more user friendly and does not require you to access your prestashop installation via FTP or SSH, I would recommend this installation method for non-technical users. If this method will fail to install module, please use manual installation.

Manual installation is more 'bullet proof' but requires some technical knowledge. It is a good installation method for people who has some technical knowledge and knows how to access prestashop installation via FTP or SSH.

## Automatic Installation Method ##

  1. Go to Downloads section and choose version of the module that matches your prestashop version.
  1. Download zip file to your local disk.
  1. The name of the downloaded file should be activationbymail\_YYYY\_MM\_DD.zip, where YYYY - year, MM - month, DD - day of the release.
  1. Go to your prestashop and login to administration panel.
  1. Go to 'modules tab'.
  1. Click 'add new module' option.
  1. Browse for activationbymail.zip file from your local disk and click 'upload this module'.
  1. If prestashop has successfully added activationbymail module you should be able to see it in 'modules tab' under Administration or Tools category. If you can not find activationbymodule there, that means that module was not successfully added, please consult official Prestashop documentation too find solution to your problem.
  1. If you can see activationbymail module under Administration or Tools category, you can click install option.
  1. After clicking install option you should see installation confirmation dialog.

## Manual Installation Method ##

  1. Connect remotely to the server using protocol that allows you transferring files, you can use FTP, SFTP, SCP or login using SSH and use wget to download module from google code.
  1. Find out the location on the remote server where your prestashop instance is installed, it can be something like /var/www/prestashop, /home/user/public\_html/prestashop, /home/user/mydomain/public\_html/prestashop etc.
  1. Download zip archive from Downloads section for your version of Prestashop
  1. Extract locally zip archive from Downloads section, you should see activationbymail folder.
  1. Upload activationbymail folder to the modules directory of prestashop directory, so the full path will be something like /home/user/public\_html/prestashop/modules/activationbymail.
  1. Go to 'module tab'.
  1. Under Administration or Tools tab find activationbymail module.
  1. Click install button.
  1. Information about successful installation should be visible in the top of the page.