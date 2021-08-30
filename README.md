# pixselect_automation
Pixselect-Test- Automation 

TESTCASE
*Automation have two test cases,

Canli Yayin İzle 
--------------
* Browserda Pixselect Sayfası acılır ve login olunur
* Canlı yayın izle butonu tıklanır
* Canlı yayın sayfasına gidilir ve kayıt izlenir
TESTCASE2
Kayit İndir 
--------------
* Browserda Pixselect Sayfası ve acılır ve login olunur
* Kayıt izle butonu tıklanır
* Kayıt izle sayfasına gidilir ve kayıt izlenir
* İstenilen kayit süresi Saat ve dakika girisi olarak yapilir
* Kayıt indirilir
* 20 saniye beklenir ve browser kapatılır.


-----Raporlama-----
Raporlama işlemi Gauge tarafından test tamamlandıktan sonra yapılır.Test failed olduysa hata kayıtları ekran görüntüsü 
şeklinde yansıtılır.Tercih edilen browserda açılır. 

--------------------

Pre Requisites
Java

Maven

Selenium

Gauge


## How to Install Gauge Core
On Windows

Install Chocolatey by executing the following command.
@"%SystemRoot%\System32\WindowsPowerShell\v1.0\powershell.exe" -NoProfile -InputFormat None -ExecutionPolicy Bypass -Command "iex ((New-Object System.Net.WebClient).DownloadString(‘https://chocolatey.org/install.ps1'))" && SET "PATH=%PATH%;%ALLUSERSPROFILE%\chocolatey\bin"

Install Gauge by executing the following command.
choco install gauge

On MacOS

Update Homebrew.
brew update

Install Gauge using Homebrew.
brew install gauge

On Linux

First, add Gauge’s GPG key with this command.
sudo apt-key adv --keyserver hkp://pool.sks-keyservers.net --recv-keys 023EDB0B

Then add Gauge to the repository list using this command.
echo deb https://dl.bintray.com/gauge/gauge-deb nightly main | sudo tee -a /etc/apt/sources.list

Finally, install Gauge using these commands.
sudo apt-get update
sudo apt-get install gauge


How to Install Gauge Plugins
Open Command Prompt and execute following commands.
gauge install java
gauge install html-report
gauge install json-report
gauge install xml-report
gauge install spectacle
gauge install flash

You can check the installation using the following command.
gauge -v

If the installation is success, it will output like this:

    Gauge version: <version number>
    Plugins
    -------
    flash (<version number>)
    html-report (<version number>)
    java (<version number>)
    json-report (<version number>)
    spectacle (<version number>)
    xml-report (<version number>)
