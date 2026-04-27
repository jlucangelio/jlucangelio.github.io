Menu: no

# Online presence

## Threat model

I am less concerned about exploitation than I am about online accounts being
disabled because some machine-learning model went haywire. My threat model,
in order of priority, is:

*   Getting locked out of the online account.
*   The online account getting exploited.

## Online acccounts

I have a vanity domain that supports email forwarding. Each of the below
categories has a separate email address at the vanity domain:

*   Financial information (banks, investments, retirements).
*   Utilities.
*   Medical.

The vanity domain forwards to a Gmail account. However, the vanity domain is not
hosted on Google, it's hosted on Namecheap. Moreover, the Namecheap account is
associated with a non-Google email account.

I'm a Google Fi customer so my phone number, and access to phone calls and SMS
is directly tied to my Gmail account.

The Gmail account has my work account as the recovery account.

## Incident response playbook

### Google account gets disabled

If my Google account were to get disabled, I would lose access to the following
services:

*   Email.
*   Phone calls and SMS.

The steps to recover would be:

*   Log in to Namecheap with username, password, and security key. No SMS 2FA
    for Namecheap.
*   Redirect all email aliases to non-Gmail email account.
*   Double-check that bank, investment, and retirement accounts can do 2FA with
    email (realistically I should check this now.)
*   Attempt to recover the Gmail account, knowing that financial information
    and utility bills are still fully accessible.

### Namecheap account gets disabled

(I find this extremely unlikely, but maybe I forget to pay the bill.)

If my Namecheap account were to get disabled, I would lose access to:

*   Email communication from bank, investment, and retirement accounts.
*   Utility bills.

The steps to recover would be:

*   Log in to each service and replace the email address with a non-forwarded
    one.
*   2FA would still be possible with a phone number, Android app confirmation,
    or security key.

### Secondary (Namecheap-associated) email account gets disabled

(Since this account is used for nothing except for Namecheap email, I also find
this extremely unlikely.)

If my secondary email account were to get disabled, I would lose access to:

*   Namecheap emails (but not Namecheap itself.)

The steps to recover would be:

*   Log in to Namecheap with username, password, and security key, and change
    the associated email address.

## TODO

### I lose my phone with the Authenticator app

### I lose all my security keys (like in a house fire)
