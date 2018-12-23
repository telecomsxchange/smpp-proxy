# smpp-b2bua
SMPP Back to Back User Agent.

TelecomsXChange SMPP B2BUA is the core component for the SMS exchange functionality on telecomsxchange platform, it handles sms routing,billing and end to end control  

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

- PREFIX LENGTH (MCC+MNC)
- Least Cost Routing. // routes according to least cost route price 
- Buyer Tech Prefix // The ability to change routes from carrier to carrier by simply pointing to a different tech prefix
- ORDER. // The ability to set order value for vendors 1,2,3 where 1 is first in route, 2 is second priority, 3 if 1&2 failed to connect.

# Billing

The SMPP B2BUA is seamlessly integrated with TelecomsXChange Billing engine with the help of Radius (AAA), Authentication, Authorization, Accouting. some of the capabilities are:

- Prepaid (Authorized to only use the available prepaid amount in account)
- Post-Paid (Credit Limit)
- Rating (According to the longest prefix "MCC+MNC")


# TESTING CHECK LIST

- InfoBIP. ----> Testing Completed successfully
- RestcommSMC ---> Testing completed successfully.
- MontyMobile ---> Testing completed successfully.
- AirTel
- TATA
- Twilio 
- SQUIRETECH
- JASMIN

# Languages Tested

- English ----> Test completed successfully  
- Arabic -----> Test completed successfully 
- Persion
- Chinese 

