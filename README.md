# MailerSendExample

This repository contains an example of how to use MailerSend (https://www.mailersend.com/)
to send emails from DBL.

Before you can use this example you will need to:

1. Create a free account with MailerSend (if you decide to use the service long
   term you may need to subscribe for an elevated service).

2. Register your internet domain name with MailerSend. This involves creating
   some TXT and CNAME records in your DNS to prove that you own the domain.

3. Apply to have your account and domain approved by MailerSend. This can only
   be done once you have confirmed domain ownership, and util approved you will
   only be able to send emails to addresses in your own domain.

4. Log in to your account, access the domain settings, and create an "API Token".
   This is essentially a secret password that you can use when making requests
   to the web service API to identify your account. The web site will only
   display the API token once, so make sure you copy it and store it somewhere
   secure for future use.

5. Record your API key in the file MailerSendApiToken.txt. You will notice this
   file in the MailerSendExample project but it is not provided by the Git
   repository. Open the file, paste your API token, press ENTER to ensure
   the record has a line terminator, then save the file. The file properties
   are set to "Copy to output directory: always" to ensure that it will always
   be in the current directory when built in Visual Studio, but in your
   application environment you will need to distribute the file yourself, or
   even better, alter the code to obtain the API token via a more secure mechanism.

Once your domain has been approved your account can be used to send 100 emails
per month. You can increase this to 3,000 per month (at the time of writing)
by subscribing to the free plan, but doing so requires you to provide credit
card details, as if you exceed the 3,000 messages you will be charged $1 per
1,000 additional messages (at the time of writing). Additional plans exist
that provide more messages, additional services, and can include sending SMS
messages if needed. You can also save money on subscriptions by paying on
an annual basis.


