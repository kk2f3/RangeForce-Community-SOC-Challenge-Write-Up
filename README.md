# RangeForce-Community-SOC-Challenge-Write-Up


# Windows - Email Challenge

The first challenge requires examination and investigation of email headers to determine if they are malicious.

Checking the source code of the first email for the IP address of the origin, and checking it in [ipinfo.io](https://ipinfo.io) reveals the company name.

![01 Email](https://user-images.githubusercontent.com/84886843/125162763-96163280-e181-11eb-915a-eadee36312d9.png)

Examining the header using G Suite revealed the SPF Status `softfail`

![02 Email](https://user-images.githubusercontent.com/84886843/125163199-f6a66f00-e183-11eb-9985-c4092dca0d77.png)

Checking the malicious looking URL `http://router-c614cfb4-a9a7-4146-85e4-deeaa38fc0da.eastus.cloudapp.azure.com/` using [urlscan.io](https://urlscan.io/) revealed that it was suspected of phishing.

![03 Email](https://user-images.githubusercontent.com/84886843/125163347-a1b72880-e184-11eb-9e5d-ab97e210a20b.png)



