# Bright Data Datacenter Proxies

[![Promo](https://github.com/luminati-io/Datacenter-Proxies/blob/main/Proxies%20and%20scrapers%20GitHub%20bonus%20banner.png)](https://brightdata.com/proxy-types/datacenter-proxies?promo=github15)

## Overview
Leverage Bright Data's extensive [datacenter proxy network](https://brightdata.com/proxy-types/datacenter-proxies) with unmatched scale and speed for reliable data collection and web scraping.

- **770,000+ Datacenter IPs**
- **[Shared](https://brightdata.com/solutions/shared-proxies) and [Dedicated](https://brightdata.com/solutions/dedicated-proxies) IP Options**
- **~0.24s Average Response Time**
- **HTTP(S) & [SOCKS5](https://brightdata.com/solutions/socks5-proxies) Support**
- **Free Country-Level Targeting**

## Key Features
- **Global Reach**: Access datacenter IPs across [98 countries](https://brightdata.com/locations).
- **High Success Rates**: Achieve up to 99.9% success in scraping tasks.
- **Fast and Reliable**: 99.99% network uptime and rapid connection speeds.
- **Customizable Options**: Choose between shared or dedicated IPs based on your needs.
- **Unlimited Scaling**: Support for concurrent sessions without restrictions.

## Pricing Plans
- **Pay As You Go**: $0.6/GB for a monthly commitment-free experience.
- **Monthly Subscriptions - Shared**:
  - **10 IPs**: $1.40/IP, $14/month + VAT.
  - **100 IPs**: $1.00/IP, $100/month + VAT.
  - **500 IPs**: $0.95/IP, $475/month + VAT.
  - **1,000 IPs**: $0.90/IP, $900/month + VAT.
  - **Enterprise Plans**: Tailored solutions for large-scale data collection.

- **Monthly Subscriptions - Dedicated**:
  - **10 IPs**: $2.20/IP, $22/month + VAT.
  - **100 IPs**: $1.70/IP, $170/month + VAT.
  - **500 IPs**: $1.50/IP, $750/month + VAT.
  - **1,000 IPs**: $1.30/IP, $1300/month + VAT.
  - **Enterprise Plans**: Tailored solutions for large-scale data collection.


- **Monthly Subscriptions - Pay/GB**:
  - $0.51/GB, $499/month + VAT.
  - $0.45/GB, $999/month + VAT.
  - $0.42/GB, $1999/month + VAT.
  - **Enterprise Plans**: Tailored solutions for large-scale data collection.

Sign up and get a dollar-for-dollar match on your first deposit, up to $500!

## Getting Started with Datacenter Proxies
1. **Start Free Trial**: No credit card required.
2. **Integration**: Manage IPs and configurations with APIs or the Bright Data Control Panel.
3. **Supported Languages**: Quick start guides available for Python, Java, C#, Node.js, and Shell.

## Code Examples

### Python

```python
import sys

# Replace '[your customerID]', 'datacenter', and '[your password]' with your actual Bright Data customer ID, zone, and password
if sys.version_info[0] == 2:
    import six
    from six.moves.urllib import request
    opener = request.build_opener(
        request.ProxyHandler(
            {'http': 'http://brd-customer-[your customerID]-zone-datacenter:"[your password]"@brd.superproxy.io:22225',
             'https': 'http://brd-customer-[your customerID]-zone-datacenter:"[your password]"@brd.superproxy.io:22225'}))
    print(opener.open('https://geo.brdtest.com/mygeo.json').read())

if sys.version_info[0] == 3:
    import urllib.request
    opener = urllib.request.build_opener(
        urllib.request.ProxyHandler(
            {'http': 'http://brd-customer-[your customerID]-zone-datacenter:"[your password]"@brd.superproxy.io:22225',
             'https': 'http://brd-customer-[your customerID]-zone-datacenter:"[your password]"@brd.superproxy.io:22225'}))
    print(opener.open('https://geo.brdtest.com/mygeo.json').read())
```

### Java

```java
package example;

import org.apache.http.HttpHost;
import org.apache.http.client.fluent.*;

public class Example {
    public static void main(String[] args) throws Exception {
        // Replace '[your customerID]' and '[your password]' with your actual credentials
        HttpHost proxy = new HttpHost("brd.superproxy.io", 22225);
        String res = Executor.newInstance()
            .auth(proxy, "brd-customer-[your customerID]-zone-datacenter", "[your password]")
            .execute(Request.Get("https://geo.brdtest.com/mygeo.json").viaProxy(proxy))
            .returnContent().asString();
        System.out.println(res);
    }
}
```

### C#

```c#
using System;
using System.Net;

class Example
{
    static void Main()
    {
        // Replace '[your customerID]' and '[your password]' with your actual credentials
        var client = new WebClient();
        client.Proxy = new WebProxy("brd.superproxy.io:22225");
        client.Proxy.Credentials = new NetworkCredential("brd-customer-[your customerID]-zone-datacenter", "[your password]");
        Console.WriteLine(client.DownloadString("https://geo.brdtest.com/mygeo.json"));
    }
}
```

### Node.js

```node.js
require('request-promise')({
    url: 'https://geo.brdtest.com/mygeo.json',
    proxy: 'http://brd-customer-[your customerID]-zone-datacenter:"[your password]"@brd.superproxy.io:22225',
    })
.then(function(data){ console.log(data); },
    function(err){ console.error(err); });
```

### Shell

```shell
# Replace '[your customerID]' and '[your password]' with your actual credentials
curl --proxy brd.superproxy.io:22225 --proxy-user brd-customer-[your customerID]-zone-residential:[your password] -k "https://geo.brdtest.com/mygeo.json"
```

## Integrations
Our datacenter proxies are compatible with popular automation tools, including:

- [**Puppeteer**](https://brightdata.com/integration/puppeteer)
- [**Selenium**](https://brightdata.com/integration/selenium)
- [**Playwright**](https://brightdata.com/integration/playwright)
- [**AdsPower**](https://brightdata.com/integration/adspower)
- [**MultiLogin**](https://brightdata.com/integration/multilogin)

## Use Cases
Common applications for datacenter proxies:

- [**eCommerce**](https://brightdata.com/use-cases/ecommerce): Track pricing and product availability.
- [**Social Media**](https://brightdata.com/use-cases/social-media-for-marketing): Monitor trends and engagement.
- [**Real Estate**](https://brightdata.com/use-cases/real-estate): Collect data on property listings.
- [**Travel**](https://brightdata.com/use-cases/travel): Compare travel deals across locations.

## FAQ

### What is a Datacenter Proxy?
Datacenter proxies provide IPs assigned to servers, allowing you to change your IP and location for web scraping and other use cases.

### What are the advantages of Datacenter Proxies?
Datacenter proxies are fast and cost-effective, ideal for simple data collection tasks, account management, and bypassing basic geo-restrictions.

### How are Datacenter Proxies used by businesses?
From competitive analysis to digital asset protection, datacenter proxies support a wide range of tasks across various industries.

### Where are Bright Data's Datacenter Proxies located?
Our proxies span 98 global locations, with high IP counts in the [USA](https://brightdata.com/locations/united-states), [Canada](https://brightdata.com/locations/ca), [UK](https://brightdata.com/locations/gb), [Germany](https://brightdata.com/locations/de), and [France](https://brightdata.com/locations/fr).

### Are Datacenter Proxies fast?
Yes, with minimal routing, datacenter proxies offer fast connections, making them optimal for time-sensitive applications.

### Should I use shared or dedicated Datacenter Proxies?
Use dedicated proxies for exclusive access or shared proxies for cost-effective solutions to common scraping and testing tasks.
