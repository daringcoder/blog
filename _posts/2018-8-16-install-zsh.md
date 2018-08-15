---
layout: post
title: উবুন্টুতে zsh শেল ইন্সটল করুন
---

লিনাক্সের জন্য zsh শেল বেশ জনপ্রিয়। খুব সহজেই অামরা উবুন্টুতে zsh শেল ইনস্টল করতে পারি। ইনস্টল করার জন্য রুট ইউজার হিসেবে এক্সেস করে প্রথমে নিচের কমান্ডটা দেব।  
{% highlight bash %}  
apt-get install zsh
{% endhighlight %}  

ইন্সটল হয়ে গেলে নিচের কমান্ডটা দেব, যাতে ডিফল্ট শেল হিসেবে zsh সেট হয়ে যায়।  
{% highlight bash %}  
chsh -s /bin/zsh
{% endhighlight %}  

এইবার রুট ইউজার থেকে লগ-অাউট করে অাবার রুট ইউজার হিসেবে লগইন করব। তাহলে zsh শেল চালু হয়ে যাবে। এখন অামরা oh-my-zsh ইন্সটল করব, যাতে অামরা Zsh এ থীম ইউজ করতে পারি। ইন্সটল করার জন্য নিচের কমান্ডটা দেব।  
{% highlight bash %}  
wget https://github.com/robbyrussell/oh-my-zsh/raw/master/tools/install.sh -O - | zsh
{% endhighlight %}  

ইন্সটল হয়ে গেলে ডিফল্ট থীম চেঞ্জ করে agnoster থীম সেট করার জন্য নিচের কমান্ডটা দেব।  
{% highlight bash}  
gedit ~/.zshrc
{% endhighlight %}  

ফাইলটা ওপেন হলে দশ নাম্বার লাইনটাকে ZSH_THEME="agnoster" লিখে রিপ্লেস করে সেভ করে ফাইলটা ক্লোজ করে দেব। এরপর নিচের কমান্ডটা দিয়ে powerline fonts ইনস্টল করব, যাতে থীমটা ঠিকমত রেন্ডার হয়।  
{% highlight bash %}  
apt-get install fonts-powerline
{% endhighlight %}  

ইন্সটল হয়ে গেলে টার্মিনালের profile preferences এ গিয়ে Colors অপশন থেকে Built-in Schemes হিসেবে Solarized dark সিলেক্ট করে দেব। এরপর রুট ইউজার থেকে লগ-অাউট করে অাবার লগইন করব। তাহলে অামরা নিচের মত সুন্দর একটা টার্মিনাল দেখতে পাবো।  
![zsh-terminal]({{ "/images/terminal.png" | absolute_url }})

