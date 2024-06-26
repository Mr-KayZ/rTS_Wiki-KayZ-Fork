---
layout: default
title: Session Hijacking
nav_exclude: false
has_children: false
parent: Safety & Security
search_exclude: false
last_modified_date: 2024-06-23
redirect_from: /books/safety-and-security/page/session-hijack
---
# Session Hijacking
{: .no_toc}

{% include toc.md %}

Session hijacking is a cyber attack where an attacker intercepts and controls a user's session with a web application. This can occur during various online activities, such as checking credit card balances or shopping. The attacker can then perform any action that the legitimate user could, leading to potential consequences like accessing sensitive information, stealing money, or committing identity theft. 

There are two types of session hijacking attacks: active, where the attacker controls the target's session while it's active, and passive, where the attacker steals the target's session ID by eavesdropping on network traffic. 

Session hijacking is dangerous as it allows attackers to gain unauthorized access to protected accounts by posing as a legitimate user. Therefore, staying informed about the latest attack techniques and prevention methods is essential.

## Active Session Hijacking and cookies
Cookies, also known as internet or HTTP cookies, are small text files that websites store on your computer. They contain data such as a username and password, which are used to identify your computer as you use a network. Cookies are generated by web servers and sent to browsers, which then include the cookies in future HTTP requests.

Cookies serve several purposes. They help inform websites about the user, enabling the websites to personalize the user experience. For example, e-commerce websites use cookies to remember what merchandise users have placed in their shopping carts. Some cookies are necessary for security purposes, such as authentication cookies.

However, cookies can also pose security and privacy concerns. Some viruses and malware may be disguised as cookies. These malicious elements can be used to facilitate session hijacking, a type of cyber attack where an attacker intercepts and takes control of a user’s session with a web application. This can be done actively, where the attacker takes control of the target’s session while it’s active, or passively, where the attacker eavesdrops on network traffic to steal the target’s session ID (Or session token).

In the context of session hijacking, viruses and other malware can be used to steal session cookies, allowing the attacker to impersonate the user and gain unauthorized access to their accounts. Third-party tracking cookies can make it easier for parties you can’t identify to watch where you’re going and what you’re doing online.

A concerning characteristic of cookies and session tokens is their persistence even after a password reset, as long as the device remains active. This means that a malicious actor could maintain access to an account and continue to cause damage, particularly if the session hijacking is facilitated by a virus. 

To mitigate this risk, it is necessary to [reinstall the operating system](/docs/installations/), followed by resetting the passwords to ensure the unauthorized user no longer has access to any accounts. Depending on the nature of the account, it may also be crucial to remove authorized devices from the account and re-enroll them, further securing the account from potential threats.

A notable instance of session hijacking occurred with the Linus Media Group, widely recognized for their YouTube channel, Linus Tech Tips (Video of their Session hijacking can be found [here](https://www.youtube.com/watch?v=yGXaAWbzl5A)). Following the download of a malicious PDF file, a virus was able to steal the session tokens, thereby gaining unauthorized access to the channel. Despite password resets, the attacker maintained access due to the possession of the session token. To effectively neutralize the threat and regain control of their accounts, it was necessary for the Linus Media Group to reinstall their operating system and subsequently reset their passwords.

## Passive Session Hijacking

Passive session hijacking occurs when an attacker eavesdrops on network traffic to steal the target’s session ID. This type of attack is easier to execute because all an attacker needs is access to network traffic, which can be easily accomplished if they are on the same network as the target. This is why it is recommended to be extra careful especially when utilizing public wifi for places, such as coffee shops and airports.

In a passive session hijacking attack, the attacker does not actively take control of the session, but rather monitors and collects data from the session. This can include sensitive information such as login credentials, personal data, and financial information.

As an end user, there are several strategies you can employ to prevent passive session hijacking:

- **Use HTTPS**: Always use websites that employ HTTPS (Hypertext Transfer Protocol Secure), which encrypts the data between your browser and the website, making it harder for attackers to eavesdrop on your sessions.
- **Use a VPN**: A Virtual Private Network (VPN) encrypts your internet connection, making it more difficult for attackers to intercept your data.
- **Log Out of Websites**: Always log out of websites when you're done using them. This ends your session, preventing attackers from hijacking it. Especially important in areas with public internet access.
- **Enable Multi-Factor Authentication**: This adds an extra layer of security, requiring another form of verification (like a text message or biometric data) in addition to your password.
- **Be Cautious of the Links You Click**: Be wary of clicking on links, especially in emails or messages, as these could lead to malicious websites designed to steal your session ID.
- **Keep Software Up to Date**: Regularly update your operating system, web browser, and other software to ensure you have the latest security patches.

## Examples of prime targets for Session Hijacking and precautions to take:

Session hijacking can potentially affect users across a wide range of commonly used services and applications. One of the best protections for session hijacking is the use of [Multi-Factor Authentication (MFA)](/docs/safety-security/mfa.md). Here are some additional examples and precautions you can take:

- **Social Media Platforms (Facebook, Twitter, Instagram, etc.)**: These platforms are prime targets for session hijacking due to the wealth of personal information available. Always log out of your sessions when finished, especially on shared devices, and consider using two-factor authentication.
- **Email Services (Gmail, Outlook, Yahoo, etc.)**: Email accounts are often linked to many other services, making them a valuable target. Use strong, unique passwords and enable two-factor authentication.
- **Online Shopping Platforms (Amazon, eBay, etc.)**: These sites have your financial information, making them attractive targets. Always ensure you're using a secure (https) connection and log out when finished.
- **Banking and Financial Services**: These are obvious targets due to the direct access to financial assets. Most banks offer two-factor authentication and other security measures — use them.
- **Cloud Storage Services (Dropbox, Google Drive, etc.)**: These services can contain a lot of personal or sensitive data. Use strong, unique passwords and two-factor authentication.
- **Video Conferencing Platforms (Zoom, Microsoft Teams, etc.)**: Unauthorized access to these can lead to eavesdropping on private conversations. Use passwords for meetings and don't share meeting links publicly.

Remember, the key to protecting yourself is vigilance. Always be aware of the information you're sharing and who you're sharing it with. Use all available security measures, such as strong, unique passwords, two-factor authentication, and secure (https) connections.

## Recommended Actions in the Event of Suspected Session Hijacking

If you suspect you are a victim of session hijacking, here are the following steps to follow:

1. **Reinstall the operating system:** If you have downloaded anything suspicious lately, then the best step is to reinstall the operating system since the session hijack could be virulent in nature. It is always safer to start from a clean slate than to stumble around while the attacker still has access to the account. Steps to reinstall an operating system can be found in our [Reinstallation wiki article](/docs/installations/).

2. **Terminate all sessions from the service:** Many services offer you to terminate sessions from any device. If you suspect one of your devices have had their session token/cookie stolen, then utilize another device and terminate the session from there. Details on how to terminate sessions from popular services can be found below.

3. **Resetting passwords, and utilizing password managers and MFA:** Last but not least. Resetting passwords may not do much during a session hijack, but it will guarantee prevention of future issues. Some services also terminate sessions immediately as well in the event of a session hijack (Steam and Discord do this), so you may not need to terminate sessions actively. Utilizing password managers to use random passwords for all accounts is also highly recommended, as it will prevent attackers from using the same password elsewhere for another account. More information on password managers can be found in our [Password Managers wiki article](/docs/safety-security/pw-managers.md). Multi-Factor authentication is an added security layer on top of that, allowing you to see potential false logins and prevent other people from accessing your account. More information on MFA can be found in our [Multi-Factor Authentication wiki article](/docs/safety-security/mfa.md).