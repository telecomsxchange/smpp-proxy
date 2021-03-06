![](https://user-images.githubusercontent.com/26701933/54167718-c5161f80-4473-11e9-82cc-f6ff64227d8e.png)

# Demo

Contact support@telecomsxchange.com or visit www.telecomsxchange.com/contact

# smpp-proxy
SMPP Proxy / B2BUA

TelecomsXChange SMPP proxy is the core component for the SMS exchange functionality on telecomsxchange platform, it handles sms Routing,Billing and security using AAA, this stack has already successfully handled (routed and billed) millions of SMS messages.

- HIGH TPS SUPPORT up to 3000/sec per node (P.S with no billing)
- SMS ROUTING/LCR
- Throttling Control per buyer/IP-account/Route
- PREPAID/POST BILLING/charging
- Concatenated Message Billing / Support
- DLRs - Delivery Report Relay
- Realtime SMS control and call data records (CDRs) generation using RADIUS
- Seamless compatibility with majority of popular SMPP software and hardware on the market today
- Robustness and Resilence
- Supports SMPP V 5.x and backward compatiable with V3.x
- SUPPORT RTL such as arabic and chinese letters
- Accurate SMPP Rate limiting per account/route

# Encodings 

This SMPP implementation supports 3 encodings: ASCII (GSM 03.38), LATIN1, and UCS2. Respective data_coding for these encodings are 0x01, 0x03, and 0x08.

Default encoding for data_coding:0 is ASCII. 






# ROUTING

The routing capabilities are: 

- [x] PREFIX LENGTH (MCC+MNC) 
- [x] Least Cost Routing :routes according to least cost route price for the longest prefix length. 
- [x] Buyer Tech Prefix: The ability to change routes from carrier to carrier by simply pointing to a different tech prefix
- [x] ORDER: The ability to set order value for vendors 1,2,3 where 1 is first in route, 2 is second priority, 3 if 1&2 failed to connect. 
- [x] Load Balancing / Weight 

# Billing

The SMPP B2BUA is seamlessly integrated with TelecomsXChange Billing engine with the help of Radius (AAA), Authentication, Authorization, Accouting. some of the capabilities are:

- Prepaid (Authorized to only use the available prepaid amount in account)
- Post-Paid (Credit Limit)
- Rating (According to the longest prefix "MCC+MNC")

# Hardware tests with billing

### 450,000,000 SMS per month.

- [x] On Dual Xeon E5-2690 v3 2.60 GHz, 30M Cache Processors (24 Cores / 48 Threads) the SMPP proxy can run 180+ messages per second with AAA (Authorization, Authentication, Accounting).

NodeJS is single threaded so to scale, you'll have to be running two SMPP proxies on same hardware will double the capacity.

# TESTING CHECK LIST

- InfoBIP. ----> Testing Completed successfully
- RestcommSMC ---> Testing completed successfully.
- MontyMobile ---> Testing completed successfully.
- AirTel  ----> Test completed successfully
- X2One ---> Test completed successfully
- Mitto.ch ---> Test completed successfully
- TATA  
- PlaySMS ----> Test completed Successfully 
- SQUIRETECH
- JASMIN ---> Test completed successfully

# Languages Tested

- English ----> Test completed successfully  
- Arabic -----> Test completed successfully 
- Chinese ----> Test completed successfully.

