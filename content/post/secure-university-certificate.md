---
author: "Rahul Sinha"
title: "Secure University Certificate and Transcript Solution"
date: 2018-02-03T18:03:44+05:30
draft: false
featured_image: "img/2018/02/pic03.jpg"
featuredalt : "Pic 3"
featuredpath : "date"
linktitle : ""
type : "post"
---

{{ with .Params.featured_image }}
  {{$fi := add ($.Site.Params.imagedir | default "img/") . }}
  <img src="{{$fi | relURL}}" alt="{{$.Params.image_alt | default "Some default description if you want it or maybe try to point to a default site param?"}}">
{{ end }}


This is Part 3 of a series of blog posts investigating university certificate fraud and potential solutions. This part provides an overview of our secure certificate generation solution and how it addresses the issues raised earlier. Part 1 explains the problem and Part 2 investigates typical solutions deployed by universities to address same.

At Qryptal, we have been working in this space for years and feel that an ideal solution to address this problem should have the following characteristics:

Should work on physical printed paper: 
Often documents are required to be be submitted in physical paper format or copies are generated for printing — making electronic digital signing solutions great in theory but not too viable in practice. This may seem counter intuitive with nearly everyone carrying a smartphone but when is the last time you submitted or verified an electronic signature?

With smartphones, often instead of scanning paper — users simply take a photo of the document and share it instantly. Electronic digital signatures get lost in this process of printing or taking “photos”. This is the practical reason why for a decade everyone has been hailing these electronic signing solutions as a panacea — which never delivered.

Easy to validate on an ad-hoc basis: 
If a solution requires many steps/equipment — it will simply not get used!
Just because you make a system available for document validation, it does not mean that it will get used. 
We technologists are guilty of this sin all the time. Often a big budget grand project is created with a lot of fanfare to solve a problem. After it finally get’s deployed — we wait and wait for usage and then finally blame the user for not “getting it”.
It is not the fault of the user — complexity inundates us everywhere and the solutions which are easy and feel intuitive are the ones which end up getting traction.
So if your mission is to make your documents trustworthy, then you have to make it super easy for anyone to validate the same without compromising on the security aspect. No messing around with visiting websites, creating accounts etc etc.
Avoid Central Database or network access to validate: 
As recent hacking news has made it clear, network based solutions can introduce their own vulnerabilities (DNS, SSL, Privacy) and attack surfaces. 
Educational Certificates are especially vulnerable because if someone sneaks in a new record for a student who apparently graduated ten years back, how will that be detected?
Perpetuators could be outside hackers or even some future disgruntled employee who thinks that this is a victimless and undetectable crime.
The Qryptal Secure Document System (QSDS) has been designed from the ground-up to provide the most elegant solution for securing university degrees and certificates.

This is how a secured certificate looks like:

The systems adds the secure Qryptal code to the certificate. Since this is a visual bar code (QR Code), it not only appears on the original but also copies: whether scanned or simple photos of the document.

Now anyone coming across this certificate can simply scan the code with the validation App and instantly verify. You can also try this right now by visiting

verify.demo-university.com

on your smartphone, installing the App and scanning the code above.

The major features of the Qryptal Secure Document System technology are:

Server-less: 
No servers, cloud or central database is required — just need the App to validate. 
Apart from security and privacy benefits, this feature also implies that once a certificate is generated and issued, that certificate stays valid and can continue to be verified without the need to maintain any infrastructure!
Tamper proof code: 
Digitally signed code uses levels of security much higher than those commonly used for internet banking (equivalent to a 3072 bit key)
Small Code Size: 
Unique compression technology keeps the code small while maintaining high levels of security
Deploying the Qryptal Secure Document System is also easy and we currently offer the following options:

Web Service API: 
This is a RESTful API where your existing document generation system can make secure API calls to our system and get the secure code or the fully generated certificate PDF based on your template.
On-premise software:
We provide you with the Qryptal Generator software that you run in-house to generate these secure codes/certificates.
MS Excel Add-in:
If you use MS Excel as a database, we have an Addin which makes it easy for your operators to just click and generate secure codes/certificates.
For more information or trial, please contact us at: