<div align="center">
<img src="images/image1.png"  width="10%">
</div>

# Simple Email Service (SES)

Amazon SES is an email platform that provides an easy, cost-effective way for
you to send and receive email using your own email addresses and domains.
Many organization has generic emails like <noreply@example.com> which is used
to send emails to users upon registration or other use-cases.

<div align="center">
<img src="images/image2.png"  width="75%">
</div>

## How email sending works in Amazon SES

- Email sender makes a request to SES to send email to recipients.
- If the request is valid, SES accepts the email.
- SES sends the message over the Internet to the recipient's receiver.

Bounce Notifications (email not exist) & Complaints (feedback) are sent back to
SES which then forwards it to the sender.

<div align="center">
<img src="images/image3.png"  width="75%">
</div>
