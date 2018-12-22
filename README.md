# smpp-b2bua
SMPP Back to Back User Agent. 

TelecomsXChange SMPP b2bua is the core component for the SMS exchange functionality on telecomsxchange platform, it handles sms routing,billing and end to end control  

- HIGH TPS SUPPORT
- SMS ROUTING/LCR
- PREPAID/POST BILLING/charging
- Realtime SmS control and call data records (CDRs) generation using RADIUS
- Seamless compatibility with majority of popular SMPP software and hardware on the market today
- Robustness and Resilence
- SUPPORT SMPP V3.x and 5.x
- SUPPORT RtL such as arabic and chinese letters
- TPS limiting per account

# Encodings 

This smpp implementation supports 3 encodings: ASCII (GSM 03.38), LATIN1, and UCS2. Respective data_coding for these encodings are 0x01, 0x03, and 0x08.

Default encoding for data_coding:0 is ASCII. 


# ROUTING

The routing capabilities plan ed are: 

- PREFIX LENGTH 
- MCC MNC
- Least Cost Routing
- Tech Prefix
- ORDER

# TESTING CHECK LIST

- InfoBIP
- RestcommSMC
- Twilio
- Monty
- SQUIRETECH
- JASMIN



