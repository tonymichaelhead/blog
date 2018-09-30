---
layout: post
title:  "Install Fleep on Linux Mint 18.3"
date:   2018-09-28 22:16:14 -0700
categories: linux mint software fleep
---
If you tried to install Fleep on your Linux Mint 18.3 distro, you may have been disappointed when the Linux installation instructions on the [official page](https://fleep.io/downloads) didn't work.

As it turns out, Fleep doesn't have an official package built for Linux Mint 18.3, but fear not! Linux Mint is based off Ubuntu, so all we need to do is add the repository for the corresponding Ubuntu package and install it. I have installed Fleep on Linux Mint 18.3, so I needed to run Fleep's official build for Ubuntu 16.04 (Xenial). The steps are as follows:

Open your terminal and paste these commands in.

{% highlight shell %}
$ curl https://fleep.io/software/linux/fleep.asc | sudo apt-key add -
$ sudo add-apt-repository "deb https://builds.fleep.ee/linux/ xenial fleep"
$ sudo apt-get update
$ sudo apt-get install fleep
{% endhighlight %}

By running the above commandss you will: 

1. Add the authentication keys for the fleep repository.

2. Add the Ubuntu repository for Fleep. If you are running Linux Mint 18.3, you will need to add the Fleep repository for Ubuntu 16.04 (Xenial). Don't worry, Mint will run it just fine ;)
 
3. Make sure you have the latest versions of all your repositories.

4. Install Fleep, and enjoy.

---  
<br>
That's it! If you enjoyed this quick tutorial or have any questions please leave a comment below.

