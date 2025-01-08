## Introduction

I enjoy creating automation templates using the platform Ansible (*by Red Hat*).

Creating Ansible Roles and Modules/Collections should help others to get started faster.

Feedback is appreciated!

GPG: [https://files.oxl.at/gpg/ansibleguy.gpg](https://files.oxl.at/gpg/ansibleguy.gpg)

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

* As security is very important in todays IT environment I'm checking my Roles and Modules/Collections for security best-practises.
* Roles and Modules will at least warn you if unsecure settings are used or will not even fail on you if you use them in an unsecure way.
* You should always use encrypted connectivity => Automation makes it **very easy** to add/generate certificates. 

### Epilog

Automation can **save time and nerves**, enables **infrastructure-as-code** (*with all it's benefits*) and **scales well**.

What are you waiting on? Automate! 😄

----

Have a nice day!
- AnsibleGuy
