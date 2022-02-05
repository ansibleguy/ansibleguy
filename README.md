## Introduction

I enjoy creating automation templates using the platform Ansible (*by Red Hat*).

Making my roles OpenSource should help other IT-Admins/-Engineers/-Enthusiasts/Developers getting their projects and infrastructure up-and-running faster.

Feedback is appreciated!

### Principles

#### 💭 User interaction
Keeping the user **interaction clean and simple**
* Per example:
  
  If a network admin wants to configure a [WireGuard VPN-Infrastructure](https://github.com/ansibleguy/infra_wireguard) he/she/... should not need to think about the role - just the abstracted topology!

* Each role should use as few 'top-level' variables as possible

  Most roles will take ONE nested variable (*dictionary*)
    
* Commonly redundant config is not accepable.
  
  The role should work its magic ✨ and handle it using inheritance, scoping and/or defaults

#### 🏷 Default = Opt-out

Preferring **opt-out** on optional features
* IT-Infrastructure is a very sensitive domain.
  
  I hate it if some role/script does more than it should.
   
  That can lead to unpredictable results!
  
* The roles allow the user to choose the features they want to opt-in.

#### 📗 Documentation

Good **documentation**
* The best tool is useless if you can not handle it..

  Documentation is the tools 'interface' and should be clean.
  
  I can't tell how often I came across a tool with a nice feature-set but could not use it as of the lack of good documentation!
  
* Transparency is key when getting to know a role.

  Examples (*config => result*) are very vital for this.
  
  Not everybody wants to run the role to see what it actually does do.


#### 🔐	Security

* My roles **WILL NOT ALLOW** unsecure configurations!

* Per example:

  Webservers as [Apache2](https://github.com/ansibleguy/infra_apache) and [Nginx](https://github.com/ansibleguy/infra_nginx) will not allow you to configure a site without using SSL!

  Automation makes it **very easy** to add/generate certificates. 

### Epilog

Automation can **save time and nerves**, enables **infrastructure-as-code** (*with all it's benefits*) and **scales well**.

What are you waiting on? Automate! 😄

----

Have a nice day!
- AnsibleGuy
