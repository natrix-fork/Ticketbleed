# Ticketbleed [![License](https://img.shields.io/github/license/mashape/apistatus.svg?maxAge=2592000)](https://raw.githubusercontent.com/EgeBalci/Ticketbleed/master/LICENSE) 
This is a go library for exploiting Ticketbleed (CVE-2016-9244) vulnerability, this library is a modified version of go's crypto/tls, it has few changes inside `handshake_client.go, tls.go, common.go` files. 



# CVE-2016-9244

Ticketbleed (CVE-2016-9244) is a software vulnerability in the TLS stack of certain F5 products that allows a remote attacker to extract up to 31 bytes of uninitialized memory at a time, which can contain any kind of random sensitive information, like in Heartbleed.

Founder: Filippo Valsorda

Finding Ticketbleed: https://blog.filippo.io/finding-ticketbleed/


VULNERABLE VERSIONS:

<table>
    <tr>
        <th>Product</th>
        <th>Version</th>
    </tr>
    <tr>
        <td>BIG-IP LTM</td>
        <td>12.0.0 - 12.1.2 & 11.4.0 - 11.6.1</td>
    </tr>
    <tr>
        <td>BIG-IP AAM</td>
        <td>12.0.0 - 12.1.2 & 11.4.0 - 11.6.1</td>
    </tr>
    <tr>
        <td>BIG-IP AFM</td>
        <td>12.0.0 - 12.1.2 & 11.4.0 - 11.6.1</td>
    </tr>
    <tr>
        <td>BIG-IP Analytics</td>
        <td>12.0.0 - 12.1.2 & 11.4.0 - 11.6.1</td>
    </tr>
    <tr>
        <td>BIG-IP APM</td>
        <td>12.0.0 - 12.1.2 & 11.4.0 - 11.6.1</td>
    </tr>
    <tr>
        <td>BIG-IP ASM</td>
        <td>12.0.0 - 12.1.2 & 11.4.0 - 11.6.1</td>
    </tr>
    <tr>
        <td>BIG-IP GTM</td>
        <td>11.4.0 - 11.6.1</td>
    </tr>
    <tr>
        <td>BIG-IP Link Controller</td>
        <td>12.0.0 - 12.1.2</td>
    </tr>
    <tr>
        <td>BIG-IP PEM</td>
        <td>12.0.0 - 12.1.2 & 11.4.0 - 11.6.1</td>
    </tr>
    <tr>
        <td>BIG-IP PSM</td>
        <td>11.4.0 - 11.4.1</td>
    </tr>
</table>