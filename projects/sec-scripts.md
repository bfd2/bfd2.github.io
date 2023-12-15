---
layout: project
type: project
image: img/script-img/ubu_icon.jpg
title: "Security Scripts"
date: 2019
published: false
labels:
  - Shell
  - VSB
summary: "A series of scripts developed to secure various operating systems."
---

These are a series of scripts that me and my team developed for the CyberPatriot cyber security competition. The main objective of the CyberPatriot competition is to secure and patch as many vulnerabilities on various operating systems in the alloted 6 hours you are given. It did a variety of things like securing and disabling ports, checking for false registry values, installing and using free and secure anti-malware software, and securing system config files amongst other things done to secure points in the competition. We wrote in shell for securing Ubuntu, Debian, and other Linux-based machines, and Visual Basic (VSB) for Windows Server, 8, and 10. Due to competition rules, I cannot share the code nor the UI used in the script.

## What I learned
What I learned from this is that Bash/shell are ultimately superior for writing script on the OS level and that VSB is a big pain in the butt. For example, changing registry values on Windows using VSB is so tedious because you have to using the path of where the registry key is and then set it. For example, setting the minimum password length to 15 on Windows goes like this:
```
My.Computer.Registry.SetValue("HKEY_LOCAL_MACHINE\SOFTWARE\Microsoft\Windows\CurrentVersion\Policies\Network\MinPwdLen", 15)
```
A very long and tedious command. Compared to Ubuntu where all you do is grep the password configuration file and set the minimum length to 15.
```
sudo grep /etc/pam.d/common-password
password        [success=1 default=ignore]      pam_unix.so obscure sha512 minlen=8
```

Now you're done. It's so much more simpler than writing that long command.

### Windows is still superior sadly.
Although Linux is way better for code development and way more secure than Windows, Windows is still superior for everyday use. It's just more conveinent since everything is developed and is on Windows compared to where Linux doesn't have the same selection of applications as their counterpart. Even if those same applicatons are on Linux, it takes a long time for updates to come out and updates aren't as frequent. It's a conundrum that a lot of developers go through, but ultimately, the laptop/development tools are used in Linux and the home PC uses Windows/MacOS depending on your preference of operating systems.