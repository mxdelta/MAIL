# MAIL
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
    mail from: <duck@duck.com>
    250 OK
    rcpt to: <nico@megabank.com>
    250 OK
////


# Недостатки SMTP

nmap-p25 --script smtp-open-relay 192.168.12.25 -v -Pn

Попытка отправки email через 192.168.2.25 на внешний адрес временной почты temp mail
sendEmail -t mail@mail.ru -f aablchkin@der.ru -s 192.168.12.25 -u alarma

nmap -p25 --script=smpt-open-relay IP_ADR -v -Pn

sendEmail -t zerfrve@gufum.com -f aadsvds@vfdvs.ru -s 192.168.12.25 -u AchtungAlarm    (отправка письма)



    Автоматизированный перебор системных пользователей
    rhosts => 192.168.119.22
    auxiliary(scanner/smtp/smpt_enum) >run
