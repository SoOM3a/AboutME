---
title: SMTP Enumeration
date: 2024-03-12 10:25:41 PM
categories: [RedTeam, Enumeration]
tags: [redteam]     # TAG names should always be lowercase
authors: [0]
media_subpath: /assets/img/services_enumerations/smtp/
---

## SMTP 
MTP stands for "Simple Mail Transfer Protocol". It is utilised to handle the sending of emails. In order to support email services, a protocol pair is required, comprising of SMTP and POP/IMAP. Together they allow the user to send outgoing mail and retrieve incoming mail, respectively.

The SMTP server performs three basic functions:
 - It verifies who is sending emails through the SMTP server.
 - It sends the outgoing mail
 - If the outgoing mail can't be delivered it sends the message back to the sender

Most people will have encountered SMTP when configuring a new email address on some third-party email clients, such as Thunderbird; as when you configure a new email client, you will need to configure the SMTP server configuration in order to send outgoing emails.
POP and IMAP

POP, or "Post Office Protocol" and IMAP, "Internet Message Access Protocol" are both email protocols who are responsible for the transfer of email between a client and a mail server. The main differences is in POP's more simplistic approach of downloading the inbox from the mail server, to the client. Where IMAP will synchronise the current inbox, with new mail on the server, downloading anything new. This means that changes to the inbox made on one computer, over IMAP, will persist if you then synchronise the inbox from another computer. The POP/IMAP server is responsible for fulfiling this process.

## How does SMTP work?

Email delivery functions much the same as the physical mail delivery system. The user will supply the email (a letter) and a service (the postal delivery service), and through a series of steps- will deliver it to the recipients inbox (postbox). The role of the SMTP server in this service, is to act as the sorting office, the email (letter) is picked up and sent to this server, which then directs it to the recipient.
We can map the journey of an email from your computer to the recipient’s like this
![smtp architecture](smtp_architecture.png)

## Enumeration 
[Hydra](../hydra/)
 

<script src="https://giscus.app/client.js"
        data-repo="SoOM3a/Blogs"
        data-repo-id="R_kgDOLebVZA"
        data-category="General"
        data-category-id="DIC_kwDOLebVZM4Cd9IX"
        data-mapping="url"
        data-strict="1"
        data-reactions-enabled="1"
        data-emit-metadata="1"
        data-input-position="top"
        data-theme="preferred_color_scheme"
        data-lang="en"
        data-loading="lazy"
        crossorigin="anonymous"
        async>
</script>