*LOGIN Update Command Line Utility*
=============


Automate Updates to LOGIN Objects via Command Line Interface
http://github.com/Automic-Community/LOGIN-Update-Command-Line-Utility

<!-- List of attached files -->
Contents of Solution Package:

						
								*LOGIN_Update.zip
								
						


Documenation and Instructions
---

<p><strong>&nbsp;</strong></p>
<p>Automatically update the content of LOGIN Objects for AWA, ARA or ASO (AE) using a simple command.</p>
<p><strong>Usage:</strong></p>
<p>1- Download and unzip all files</p>
<p>2- Unzip LOGIN_Update.zip &amp; rename the connection.config.template to connection.config</p>
<p>3- Modify content of connection.config</p>
<p>4- use the command line (options available with parameter -h)</p>
<p>&nbsp;</p>
<p><strong>Usage Examples:</strong></p>
<h4 style="box-sizing: border-box; margin-top: 24px; margin-bottom: 16px; font-size: 16px; line-height: 1.25; color: #333333; font-family: -apple-system, BlinkMacSystemFont, 'Segoe UI', Helvetica, Arial, sans-serif, 'Apple Color Emoji', 'Segoe UI Emoji', 'Segoe UI Symbol';">Add a login entry to all LOGIN objects matching LOGIN.TEST*:</h4>
<p style="box-sizing: border-box; margin-top: 0px; margin-bottom: 16px; color: #333333; font-family: -apple-system, BlinkMacSystemFont, 'Segoe UI', Helvetica, Arial, sans-serif, 'Apple Color Emoji', 'Segoe UI Emoji', 'Segoe UI Symbol'; font-size: 16px;"><code style="box-sizing: border-box; font-family: Consolas, 'Liberation Mono', Menlo, Courier, monospace; font-size: 13.6px; padding: 0.2em 0px; margin: 0px; background-color: rgba(0, 0, 0, 0.0392157); border-radius: 3px;">java -jar LOGIN_Update.jar -name "LOGIN.TEST*" -u_addlogin "['WIN99','WINDOWS','admin','pwd']"</code></p>
<h4 style="box-sizing: border-box; margin-top: 24px; margin-bottom: 16px; font-size: 16px; line-height: 1.25; color: #333333; font-family: -apple-system, BlinkMacSystemFont, 'Segoe UI', Helvetica, Arial, sans-serif, 'Apple Color Emoji', 'Segoe UI Emoji', 'Segoe UI Symbol';"><a id="user-content-update-a-login-entry-to-all-login-objects-matching-logintest" class="anchor" style="box-sizing: border-box; background-color: transparent; color: #4078c0; text-decoration: none; float: left; padding-right: 4px; margin-left: -20px; line-height: 1;" href="https://github.com/brendanSapience/UC4-Automic-AE-CLI-Binary-Repository/wiki/LOGIN_Update.jar#update-a-login-entry-to-all-login-objects-matching-logintest"></a>Update a login entry to all LOGIN objects matching LOGIN.TEST*:</h4>
<p style="box-sizing: border-box; margin-top: 0px; color: #333333; font-family: -apple-system, BlinkMacSystemFont, 'Segoe UI', Helvetica, Arial, sans-serif, 'Apple Color Emoji', 'Segoe UI Emoji', 'Segoe UI Symbol'; font-size: 16px; margin-bottom: 0px !important;"><code style="box-sizing: border-box; font-family: Consolas, 'Liberation Mono', Menlo, Courier, monospace; font-size: 13.6px; padding: 0.2em 0px; margin: 0px; background-color: rgba(0, 0, 0, 0.0392157); border-radius: 3px;">java -jar LOGIN_Update.jar -name "LOGIN.TEST*" -u_updloginsrc "['WIN99','WINDOWS','admin']" -u_updlogintrg "['WIN99','WINDOWS','newadmin','password']" -commit</code></p>
<p style="box-sizing: border-box; margin-top: 0px; color: #333333; font-family: -apple-system, BlinkMacSystemFont, 'Segoe UI', Helvetica, Arial, sans-serif, 'Apple Color Emoji', 'Segoe UI Emoji', 'Segoe UI Symbol'; font-size: 16px; margin-bottom: 0px !important;">&nbsp;</p>
<p style="box-sizing: border-box; margin-top: 0px; color: #333333; font-family: -apple-system, BlinkMacSystemFont, 'Segoe UI', Helvetica, Arial, sans-serif, 'Apple Color Emoji', 'Segoe UI Emoji', 'Segoe UI Symbol'; font-size: 16px; margin-bottom: 0px !important;">Other:</p>
<p style="box-sizing: border-box; margin-top: 0px; color: #333333; font-family: -apple-system, BlinkMacSystemFont, 'Segoe UI', Helvetica, Arial, sans-serif, 'Apple Color Emoji', 'Segoe UI Emoji', 'Segoe UI Symbol'; font-size: 16px; margin-bottom: 0px !important;">&nbsp;</p>
<p style="box-sizing: border-box; margin-top: 0px; color: #333333; font-family: -apple-system, BlinkMacSystemFont, 'Segoe UI', Helvetica, Arial, sans-serif, 'Apple Color Emoji', 'Segoe UI Emoji', 'Segoe UI Symbol'; font-size: 16px; margin-bottom: 0px !important;"><em>All parameters available can be shown using the parameter -h:</em></p>
<p style="box-sizing: border-box; margin-top: 0px; color: #333333; font-family: -apple-system, BlinkMacSystemFont, 'Segoe UI', Helvetica, Arial, sans-serif, 'Apple Color Emoji', 'Segoe UI Emoji', 'Segoe UI Symbol'; font-size: 16px; margin-bottom: 0px !important;">&nbsp;</p>
<p style="box-sizing: border-box; margin-top: 0px; color: #333333; font-family: -apple-system, BlinkMacSystemFont, 'Segoe UI', Helvetica, Arial, sans-serif, 'Apple Color Emoji', 'Segoe UI Emoji', 'Segoe UI Symbol'; font-size: 16px; margin-bottom: 0px !important;">java -jar LOGIN_Update.jar -h</p>
<p style="box-sizing: border-box; margin-top: 0px; color: #333333; font-family: -apple-system, BlinkMacSystemFont, 'Segoe UI', Helvetica, Arial, sans-serif, 'Apple Color Emoji', 'Segoe UI Emoji', 'Segoe UI Symbol'; font-size: 16px; margin-bottom: 0px !important;">&nbsp;</p>
<p style="box-sizing: border-box; margin-top: 0px; color: #333333; font-family: -apple-system, BlinkMacSystemFont, 'Segoe UI', Helvetica, Arial, sans-serif, 'Apple Color Emoji', 'Segoe UI Emoji', 'Segoe UI Symbol'; font-size: 16px; margin-bottom: 0px !important;"><em>you can also use connection parameters in command line to specify which system to connect to:</em></p>
<p style="box-sizing: border-box; margin-top: 0px; color: #333333; font-family: -apple-system, BlinkMacSystemFont, 'Segoe UI', Helvetica, Arial, sans-serif, 'Apple Color Emoji', 'Segoe UI Emoji', 'Segoe UI Symbol'; font-size: 16px; margin-bottom: 0px !important;">&nbsp;</p>
<p style="box-sizing: border-box; margin-top: 0px; color: #333333; font-family: -apple-system, BlinkMacSystemFont, 'Segoe UI', Helvetica, Arial, sans-serif, 'Apple Color Emoji', 'Segoe UI Emoji', 'Segoe UI Symbol'; font-size: 16px; margin-bottom: 0px !important;">-C (Client)</p>
<p style="box-sizing: border-box; margin-top: 0px; color: #333333; font-family: -apple-system, BlinkMacSystemFont, 'Segoe UI', Helvetica, Arial, sans-serif, 'Apple Color Emoji', 'Segoe UI Emoji', 'Segoe UI Symbol'; font-size: 16px; margin-bottom: 0px !important;">-L (Login)</p>
<p style="box-sizing: border-box; margin-top: 0px; color: #333333; font-family: -apple-system, BlinkMacSystemFont, 'Segoe UI', Helvetica, Arial, sans-serif, 'Apple Color Emoji', 'Segoe UI Emoji', 'Segoe UI Symbol'; font-size: 16px; margin-bottom: 0px !important;">-W (Password)</p>
<p style="box-sizing: border-box; margin-top: 0px; color: #333333; font-family: -apple-system, BlinkMacSystemFont, 'Segoe UI', Helvetica, Arial, sans-serif, 'Apple Color Emoji', 'Segoe UI Emoji', 'Segoe UI Symbol'; font-size: 16px; margin-bottom: 0px !important;">-D (Department)</p>
<p style="box-sizing: border-box; margin-top: 0px; color: #333333; font-family: -apple-system, BlinkMacSystemFont, 'Segoe UI', Helvetica, Arial, sans-serif, 'Apple Color Emoji', 'Segoe UI Emoji', 'Segoe UI Symbol'; font-size: 16px; margin-bottom: 0px !important;">-H (Hostname of AE)</p>
<p style="box-sizing: border-box; margin-top: 0px; color: #333333; font-family: -apple-system, BlinkMacSystemFont, 'Segoe UI', Helvetica, Arial, sans-serif, 'Apple Color Emoji', 'Segoe UI Emoji', 'Segoe UI Symbol'; font-size: 16px; margin-bottom: 0px !important;">-P (Port)</p>
<p style="box-sizing: border-box; margin-top: 0px; color: #333333; font-family: -apple-system, BlinkMacSystemFont, 'Segoe UI', Helvetica, Arial, sans-serif, 'Apple Color Emoji', 'Segoe UI Emoji', 'Segoe UI Symbol'; font-size: 16px; margin-bottom: 0px !important;">&nbsp;</p>
<p style="box-sizing: border-box; margin-top: 0px; color: #333333; font-family: -apple-system, BlinkMacSystemFont, 'Segoe UI', Helvetica, Arial, sans-serif, 'Apple Color Emoji', 'Segoe UI Emoji', 'Segoe UI Symbol'; font-size: 16px; margin-bottom: 0px !important;">This binary is part of a larger kit: Additional Binaries to modify other objects can be found here:</p>
<p style="box-sizing: border-box; margin-top: 0px; color: #333333; font-family: -apple-system, BlinkMacSystemFont, 'Segoe UI', Helvetica, Arial, sans-serif, 'Apple Color Emoji', 'Segoe UI Emoji', 'Segoe UI Symbol'; font-size: 16px; margin-bottom: 0px !important;">&nbsp;</p>
<p style="box-sizing: border-box; margin-top: 0px; margin-bottom: 0px !important;"><span><span>https://github.com/brendanSapience/UC4-Automic-AE-CLI-Binary-Repository</span></span></p>
<p style="box-sizing: border-box; margin-top: 0px; color: #333333; font-family: -apple-system, BlinkMacSystemFont, 'Segoe UI', Helvetica, Arial, sans-serif, 'Apple Color Emoji', 'Segoe UI Emoji', 'Segoe UI Symbol'; font-size: 16px; margin-bottom: 0px !important;">&nbsp;</p>
<p style="box-sizing: border-box; margin-top: 0px; color: #333333; font-family: -apple-system, BlinkMacSystemFont, 'Segoe UI', Helvetica, Arial, sans-serif, 'Apple Color Emoji', 'Segoe UI Emoji', 'Segoe UI Symbol'; font-size: 16px; margin-bottom: 0px !important;">&nbsp;</p>

Copyright and License
---

Broadcom does not support, maintain or warrant Solutions, Templates, Actions and any other content published on the Community and is subject to Broadcom Community [Terms and Conditions](https://community.broadcom.com/termsandconditions)


Questions or Need Help? 
---
Join the [Automic Community Integrations](https://community.broadcom.com/communities/community-home?CommunityKey=83e49dd4-b93e-464a-a343-2bb1e51c13ec) to discuss this integration.
