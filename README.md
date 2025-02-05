# MAIL
  Отправка по smtp
  
  swaks --from amra@axlle.htb --to accounts@axlle.htb --body "Hello" --header "Hello" --attach @test.xll

  swaks -s 10.10.11.21 -f maxxxx@axlle.htb -t accounts@axlle.htb --attach @test.xll


///
telnet 10.10.10.77 25
Trying 10.10.10.77...
Connected to 10.10.10.77.
Escape character is '^]'.
220 Mail Service ready
hello ppp.htb
503 Bad sequence of commands
HELLO plessd.htb
503 Bad sequence of commands
helo bab.htb
250 Hello.
MAIL FROM <fuck@fuck.com>
550 Invalid syntax. Syntax should be MAIL FROM:<mailbox@domain>[crlf]
mail from: <fuck@fuck.com>
250 OK
rcpt to: <nico@megabank.com>
250 OK
////
