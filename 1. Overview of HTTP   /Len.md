# Chapter 1



## Summary

### 전반적인 개론의 HTTP

#### 1.3 Resources

- Media Types  
  MIME type. (Multipurpose Internet Mail Extensions)
  Web상에서 전송되는 Object 의 포맷을 태깅한다.

- URIs  
  각각의 서버 리소스는 이름을 가지고있다. 여기서 서버 리소스 이름음 Uniform resource identifier / URI 라고 한다.  
  URIs는 마치 우편주소와 같다.

  > URI는 URL 및 URN이라는 두 가지 형태로 제공됩니다.

- URLs  
  The uniform resource locator 는 가장 흔한 resource identifier 이다.  
  URL는 특별한 서버의 특정 위치를 설명한다.

- URNs  
  the uniform resource name / URN 은 content의 특정 조각들의 유니크한 이름의 역할을 한다. 2장에서 더 설명할 것!

  > Urn:ietf:rfc:2141

#### 1.4 Transactions

> GET /specials/saw-blade.gif HTTP/1.0
> Host: www.joes-hardware.com

- Methods
- Status Codes

#### 1.5 Messages

HTTP 구성

```
Start line

Header fields

Body
```

#### 1.6 Connections

- TCP / IP
  HTTP는 Application 층. nitty-gritty 핵심  
  \- Error-free data transportation  
  \- In-order delivery(데이터가 항상 순서에 맞에 받아질것이다.)  
  \- Unsegmented data stream(can dribble out data in any size at any time)

- Connections, IP Addresses, And Port Numbers

  How a brower uses HTTP to display a simple HTML resource that resides on a distant server
  \(a) The Brower extracts the server's hostname from the URL.

  \(b) The Brower converts the server's hostname into the server's IP address.

  \(c) The Brower extracts the port number(if any) from the URL

  \(d) The Brower establishes a TCP connection with the web server

  \(e) The Brower sends an HTTP request message to the server

  \(f) The server sends an HTTP response back to the browser

  \(g) The connection is closed, and the brower displays the documents

#### 1.7 Protocol Versions

- HTTP/0.9
  
- HTTP/1.0
  
- HTTP/1.0+
  
- HTTP/1.1
  
- HTTP/2.0
  

#### 1.8 Architectural Components of the Web

- Proxies  
  HTTP intermediaries that sit between clients and servers

  Web 보안을 위해서 중요한 부분이다. 클라와 서버 사이에서 존재하며 클라에서 보낸 Request를 모두 받고 이걸 relaying (전달) 한다.  
  프록시는 종종 보안을 위해 사용된다. 또한 필터 역할도 함

- Caches  
  HTTP storehouse that keep copies of popual web pages close to clients  
  A web cache or caching proxy 는 특별한 타입의 HTTP proxy server로서 특정 문서들의 복사를 유지한다.

- Gateways  
  Spcial web servers that connect to other applications  
  서버들 사이에서의 intermediaries 하는 특별한 서버들이다.

- Tunnels  
  Speical proxies that blindly forward HTTP communications.  
  HTTP application 계층으로, blindly 하게 raw데이터를 전송한다.  
  하나의 유명한 HTTP tunnels은 Secure Sockets layer traffic through an HTTP connection.

- Agents  
  Semi-intelligent web clients that make automated HTTP requests



## Important

이곳에서는 전반적인 서문에 대한 설명이 다분해서 중요하지 않는 부분은 없었다.

그래도 하나 꼽는다면 Web의 Components.

그리고 어떻게 인터넷에 접속해서 동작하는지 - DNS 관련

