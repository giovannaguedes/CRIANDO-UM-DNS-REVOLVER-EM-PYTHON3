# CRIANDO-UM-DNS-REVOLVER-EM-PYTHON3
código permite passar o host um domínio e ele tras o ip utilizando a ferramenta gethostbyname.

⚠️ Uso exclusivo para fins educacionais • Desenvolvido por M!ss s3c

📝 Guia: Criando e executando seu primeiro DNS Resolver em Python

1. Criar o arquivo do script

No terminal, crie o arquivo:

nano script8.1.py

2. Adicionar o código Python

Cole o seguinte código:

#!/usr/bin/python3
# DNS Resolver Educacional em Python
# Uso: python3 script8.1.py <domínio>

import socket
import sys

# Verifica se o domínio foi passado como argumento
if len(sys.argv) != 2:
    print("Uso: python3 script8.1.py <domínio>")
    sys.exit(1)

host = sys.argv[1]

# Retorna o IP correspondente ao domínio
print(f"{host} ---> {socket.gethostbyname(host)}")


⚠️ Observação: Este script é apenas para fins educativos e não deve ser usado para coleta de informações sem autorização.

3. Executar o script
python3 script8.1.py example.com

4. Exemplo de execução
example.com ---> 93.184.216.34

👉 O que você aprendeu aqui

socket.gethostbyname() → resolve o domínio para o IP.

sys.argv → captura argumentos passados pela linha de comando.

len(sys.argv) → valida a quantidade de argumentos fornecidos.

sys.exit() → encerra o script quando necessário.
