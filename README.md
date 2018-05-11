# WAnD_Web
Wand Web Interface to have energy visualisation

## Refer

Source code :  https://github.com/emoncms/emoncms

Linux Installation procedure : https://github.com/emoncms/emoncms/blob/master/docs/LinuxInstall.md

**Other than above things we need to consider following things as well:**

1.Install Modules like Graph,Dashboard,Group,apps,emailreport and myhomeenergyplanner, etc.

2.The first registered user will be considered as a admin.

3.Admin will have access to update the database in webserver adminstration page ( if we did any change in the server PC then we need to 
  update the database in admin page ex:http://wand.intracworks.com/emoncms/admin/view )
  
4.Admin page will have logger info as well , which shows if anything went wrong or error in server.To enable logger or debugger

  $touch /var/log/emoncms.log
  
  $chmod 666 /var/log/emoncms.log
  
5.Edit the settings.php 

  $themecolor = "standard"; 
  
  $enable_multi_user = true; 
  
  $enable_password_reset = true; 
  
  $feedviewpath = "graph/"; 
  
  change smtp details to send mail + check whether the SMTP is enabled in server PC.

### Change required to customise the icon and name

Theme\basic\   (cutomise the png or image files)

Theme\basic\theme.php (chnage name and powered by + remove release and version)

Theme\basic\embed.php (name)

Theme\basic\emon-standard.css (footer color )

Modules\user\login_block.php (change login page padding)



