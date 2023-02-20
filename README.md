commit init 내용

-> 기존 net/smtp 에서 수정 사항은 아래와 같다.

SendMail 함수의 아래 코드를 변경하였다.

config := &tls.Config{ServerName: c.serverName}

config := &tls.Config{ServerName: c.serverName, InsecureSkipVerify: true}
