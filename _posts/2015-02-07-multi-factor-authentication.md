---
layout: post
title: Factor In Some Authentication 
cover: cover.jpg
---

Very simply, multi-factor authentication (hereafter referred to as MFA) is an 
access control system. In English, this means its a system which lets you 
(and only you) into your account while simultaneously keeping everyone else out.

Simple, right?

MFA is one of many access control systems. The fundamental idea behind this 
mechnism is that if a user wishes to gain access to a specific 
electronic resource 
(e.g. a secure session on an email provider's website, or their online banking 
control panel) they must provide verification of at least two of the three 
follow
ing factors:

1. Knowledge Factors: Some datum which only the relevant user knows, (e.g. a string
 of characters comprising a password, the name of a person's favourite 
 elementary school teacher)
2. Possession Factors: Some datum which only the relevant user has 
(e.g. a house key, a USB drive, a decryption key)
3. Inheritance Factors: Some datum which only the relevant user is or which is 
inherently
part of the user themselves (e.g. a fingerprint, an iris pattern)

The justification for this mechanism is really quite simple, namely that a 
malicious
person wishing to gain unauthorized access to another user's private account
would need to attack the integrity of more than one factor. It appears to 
follow
that the greater the amount of independent factors required to access an 
account,
 the greater the difficulty in gaining unauthorized access.

Multi-factor authentication has been used regularly in authentication schemes 
within
 the mainstream market for quite some time now. A ubiquitous example of 
 multi-ffactor authentication that have penetrated mainstream martkets is the 
authentication scheme used by most
ATMs worldwide. Typically to gain authorized access to your bank account by 
way of an ATM you're required to insert your bank card (posession factor)
as well as to enter a 
secret PIN(knowledge factor).

It's important to note that it can sometimes be difficult to differentiate 
between
systems that seem to offer multi factor authentication but actually provide two
instances of the same factor. Confused yet? Here's an example that should 
clarify
things. Many online banking websites require that you enter your password and
then to answer one or more secret questions. This is not multi-factor 
authentication as both of these are knowledge factors (something the user knows)
. It has
 been shown^1 that two instances of a single factor cannot bring the same level
 of security as two instances of two independent authentication factors.

Now, why should we care? The answer is that despite the fact that MFA has been 
around
for quite some time, it's only recently that the web industry at large has
 offered multi-factor authentication to their users at no additional cost. Some 
examples include:

1. [Google](https://www.google.com/url?sa=t&rct=j&q=&esrc=s&source=web&cd=1&cad=rja&uact=8&ved=0CCsQFjAA&url=https%3A%2F%2Fwww.google.com%2Flanding%2F2step%2F&ei=F0jvVOftA8v8sAS1_oKACg&usg=AFQjCNG6jjmfJ4pLtmzI6qJygjqRXzuFhw&bvm=bv.86956481,d.cWc)
2. [Github](https://www.google.com/url?sa=t&rct=j&q=&esrc=s&source=web&cd=1&cad=rja&uact=8&ved=0CB0QFjAA&url=https%3A%2F%2Fhelp.github.com%2Farticles%2Fabout-two-factor-authentication%2F&ei=MUjvVPrHCve_sQSfnYHgAQ&usg=AFQjCNHs9onsPDDjuY0LigUgXfh69A0laQ&bvm=bv.86956481,d.cWc)
3. [Twitter](https://www.google.com/url?sa=t&rct=j&q=&esrc=s&source=web&cd=2&cad=rja&uact=8&ved=0CCQQFjAB&url=https%3A%2F%2Fblog.twitter.com%2F2013%2Fgetting-started-with-login-verification&ei=P0jvVNr2C-nksATNooKIBg&usg=AFQjCNGpyWq4rgFFBHnntYQVTC6l7xKadg&bvm=bv.86956481,d.cWc)
4. [Paypal](https://www.paypal.com/us/cgi-bin?cmd=xpt/Marketing_CommandDriven/securitycenter/PayPalSecurityKey-outside&bn_r=o)

Most of these examples involve sending a one-time use passcode within a text 
message to your mobile phone (the exception is PayPal which actually 
offers a physical card you can carry around). Then, you'll have to enter this 
code before you're
granted access to your account. The thinking here is that as your phone is 
something which you possess, entering the passcode that was sent to your phone
provides a possession factor. Suppose a determined 
attacker
was able to guess your password, they wouldn't be able to use it to leverage
 access to your precious private account unless they also have access to your 
 (unlocked) mobile phone. Conversely, if they were able to somehow steal your 
mobile phone, they would still have to guess your super-secure (heh..) password.

In general, I tend to prefer enabling multi-factor authentication wherever 
possible. Despite the fact that I'm an advocate of strong password policies, 
I don't 
have to worry as much about securing and regenerating my passwords so long as I 
have physical access to my mobile phone. In addition, revoking the second factor
device seems to be easy enough from provider to provider.

It should be noted that despite the added security that may apparently be introd
uced by enabling MFA for your account, there are still some vulnerabilities to b
e aware of. For instance, SMS-based token transmission is still susceptible to m
an-in-the-middle attacks, whereby a determined attacker (or law enforcement) wou
ld intercept a text-message destined for your mobile phone. This is why 
traditional password strength measures are still king.

Take-aways:

1. Multi-factor authentication is a thing
2. If you can afford to use it, it should, it'll make your life easier and is worth
 the initial setup time
3. Enabling MFA isn't an excuse for lax security protocols and remaining uninformed.
4. It's critical to review the specific details of each service provider's offeri
ng of MFA and to understand the limits and safeguards associated with each.
