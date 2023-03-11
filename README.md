# CEPHAS
$ dig WWW.CEPHAS.W3SPACE.COM +nostats +nocomments +nocmd
    > ;WWW.CEPHAS.W3SPACE.COM.                    IN      A
    > WWW.CEPHAS.W3SPACE.COM.             3592    IN      CNAME   YOUR-USERNAME.github.io.
    > YOUR-USERNAME.github.io.      43192   IN      CNAME   GITHUB-PAGES-SERVER .
    > GITHUB-PAGES-SERVER .         22      IN      A       192.0.2.1

// records, point your apex domain to the IP addresses for GitHub Pages.
//
185.199.108.153
185.199.109.153
185.199.110.153
185.199.111.153

// records, point your apex domain to the IP addresses for GitHub Pages.
//
2606:50c0:8000::153
2606:50c0:8001::153
2606:50c0:8002::153
2606:50c0:8003::153

// records.
//
$ dig CEPHAS.W3SPACE.COM +noall +answer -t A
> CEPHAS.W3SPACE.COM    3600    IN A     185.199.108.153
> CEPHAS.W3SPACE.COM    3600    IN A     185.199.109.153
> CEPHAS.W3SPACE.COM    3600    IN A     185.199.110.153
> CEPHAS.W3SPACE.COM    3600    IN A     185.199.111.153

// records.
//
$ dig EXAMPLE.COM +noall +answer -t AAAA
> CEPHAS.W3SPACE.COM     3600    IN AAAA     2606:50c0:8000::153
> CEPHAS.W3SPACE.COM     3600    IN AAAA     2606:50c0:8001::153
> CEPHAS.W3SPACE.COM     3600    IN AAAA     2606:50c0:8002::153
> CEPHAS.W3SPACE.COM     3600    IN AAAA     2606:50c0:8003::153

// subdomain variant.
//
$ dig WWW.CEPHAS.W3SPACE.COM +nostats +nocomments +nocmd
    > ;WWW.CEPHAS.W3SPACE.COM                     IN      A
    > WWW.CEPHAS.W3SPACE.COM.              3592    IN      CNAME   YOUR-USERNAME.github.io.
    > YOUR-USERNAME.github.io.      43192   IN      CNAME   GITHUB-PAGES-SERVER.
    > GITHUB-PAGES-SERVER.         22      IN      A       192.0.2.1
