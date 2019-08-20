# Chocolatey: Install_With_PackageManager
Software Development involves installing of various supporting softwares like servers, build tools,IDE etc. Installing software in Linux OS has become very easy with package managers like yum and apt-get. <b>Chocolatey</b> is a software package manager for windows which helps in installing software with ease.
<a id="installChoco" name="installChoco"><h3>Install chocolatey with PowerShell.exe</h3></a>
Search for PowerShell and open in administrator mode and copy the following command <br>
<code>Get-ExecutionPolicy</code><br>
If it returns Restricted, then run  the following command<br>
<code>Set-ExecutionPolicy AllSigned</code> <br>
or<br>
<code>Set-ExecutionPolicy Bypass -Scope Process</code><br>

Now run the following command:   (copy command text)<br>
<code>Set-ExecutionPolicy Bypass -Scope Process -Force; iex ((New-Object System.Net.WebClient).DownloadString('https://chocolatey.org/install.ps1'))</code>
<h4>Additional considerations</h4>
NOTE: Please inspect https://chocolatey.org/install.ps1 prior to running any of these scripts to ensure safety. We already know it's safe, but you should verify the security and contents of any script from the internet you are not familiar with. All of these scripts download a remote PowerShell script and execute it on your machine.
<h3>Note: chocolatey is a Package manager that helps developers to install most of the software with very less effort,
for instance using powershell you can type the following command and install maven
<code>choco install maven</code> and maven will be installed and all the environment variables will be set as well.
<br> Link to know what you can install using chocolatey: https://chocolatey.org/search <br>
