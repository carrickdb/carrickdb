You forgot how to update your website, didn't you? Of course you did. Let's remember how to do that, shall we?


## Signing in

Go to https://carrickbartle.com/cpanel
username: carrefpe


## How do I look at the files???

Click on "File Manager"

## Where the fuck is everything?

In "www," whatever that is (same as public_html?).

## How do I change things??

Click "Upload" on the top menu bar.

## How do I shell into the server?!?!
ssh carrefpe@carrickbartle.com -p 21098


## To install a cert

Get validation file (should be instructions about where it is in email?? idk, I had to ask customer service and they sent me a link)
Put the validation file in public_html/.well-known/pki-validation

Inform the overlords that I've done this somehow and they'll send me a .crt and bundle.

An abridged version of the instructions here now follows:
https://www.namecheap.com/support/knowledgebase/article.aspx/9418/33/installing-an-ssl-certificate-on-your-server-using-cpanel

1. Click the SSL/TLS icon.
2. Click Manage SSL Sites under Install and Manage SSL for your website (HTTPS)
3. Open the .crt file in a text file and copypaste it into the `Certificate: (CRT)` field.
This might result in a warning that the domain isn't right or something. Ignore it.
4. Click Autofill by Certificate. This will populate the other fields.
5. Click "Install Certificate."
6. Check the website for the updated cert (it may take a few minutes to update).


## Sign into My Namecheap SSL plugin (?!)

Log out in the plugin itself (where it says "carrickdb" in the small window), not cPanel.
