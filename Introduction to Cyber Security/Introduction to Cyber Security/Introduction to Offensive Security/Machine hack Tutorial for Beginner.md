+ GoBuster 
  - brute-force a website to find hidden directories and pages 
  - take a list of potential page or directory names and try accessing a website with each of them; if the pages exist, it will tell u

Ex: `gobuster -u http://fakebank.com -w wordlist.txt dir`
`gobuster -u <the website link> -w <txt file> dir`

- u: used to state the website we 're scanning
- w: take a list of words to iterate through to find hidden pages.
