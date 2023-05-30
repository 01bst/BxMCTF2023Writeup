# BxMCTF2023Writeup
This is a few writeup for BxMCTF2023


Category : General 

1. Welcome to BxMCTF

![image](https://github.com/zer00neops/BxMCTF2023Writeup/assets/103404282/3ba6b39a-5e81-4362-9f1b-4777806be6ab)

The Flag is already provided : ctf{check_out_our_sponsors!}

2. New Website 

![image](https://github.com/zer00neops/BxMCTF2023Writeup/assets/103404282/14d93541-ddac-4c7b-b991-217a89f18701)

* The error message "DNS_PROBE_FINISHED_NXDOMAIN" typically appears in web browsers when there is a DNS (Domain Name System) resolution failure. It indicates that the DNS server was unable to resolve the domain name you entered into the browser's address bar.
* So maybe, there is previous record for the url. 
* Let use online dns checker tools : https://dnschecker.org/
* Insert your domain (url). 
* It will return a few of result.
* Scroll until you see the "TXT" record  that also contain the flag. 

![image](https://github.com/zer00neops/BxMCTF2023Writeup/assets/103404282/e032a630-315f-4594-be64-e7d1762f686b)


Category : Web 

1. Blank space - I mean Page 

![image](https://github.com/zer00neops/BxMCTF2023Writeup/assets/103404282/1f3791ee-c4f6-4dbb-8d3b-ea4e886ac504)

* Visit the link given in the problem statement and it is just a blank page. 

![image](https://github.com/zer00neops/BxMCTF2023Writeup/assets/103404282/6d43facd-9476-4db6-92d3-6b0f9d4eff17)

* The first think that come to my mind when come to a blank page, is robots.txt or source code 
* Lucky for me, when i search for the robots.txt file. I got this : 

![image](https://github.com/zer00neops/BxMCTF2023Writeup/assets/103404282/e01043fe-7b07-44fe-8012-736969557e77)

* {/very-secretly-hidden}, let put in the url shall we? https://bxmweb1.jonathanw.dev/very-secretly-hidden/. 
* Boom ! you get the flag. 

![image](https://github.com/zer00neops/BxMCTF2023Writeup/assets/103404282/46225df6-25ba-472e-b086-22e1fc48079e)


2. Respository Security 

![image](https://github.com/zer00neops/BxMCTF2023Writeup/assets/103404282/5272771b-60d6-43a2-be59-decefa975a82)

* The website provided when you launch the instance i just a website to login. you need to find the credentials.
* To find the credentials, Download the web2.zip file provided.
* Once you opened the web2.zip file, it will contain a few file : 

![image](https://github.com/zer00neops/BxMCTF2023Writeup/assets/103404282/bcfd174e-f1d0-49e0-ad9d-2e4a6e7e76b8)

* Let investigate all of the file and code, who knows it will contain the credentials.
* On file called "app.py", you can see at the line 5, state my_users and have a list of username and password : 

![image](https://github.com/zer00neops/BxMCTF2023Writeup/assets/103404282/6d969547-697b-44f0-a362-411c286f3bdf)

* Let try to use it, to log in into the web 
* Here i use username : chuck and password : norris. 
* Boom! succesful to login, then happily click the secret page on the nav bar of the website and you can view the flag

![image](https://github.com/zer00neops/BxMCTF2023Writeup/assets/103404282/b48a3735-8728-4905-a932-9e8984ac39fc)












