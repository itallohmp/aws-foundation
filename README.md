Bom dia, pessoal!

Montei uma arquitetura simples no draw.io pra simular um sistema web na AWS. A ideia é a seguinte: o cliente acessa a página estática hospedada no S3 e faz a requisição de cadastro. A API recebe os dados, valida e processa o que foi enviado. O tráfego passa pelo Load Balancer para distribuir a carga e evitar sobrecarregar os servidores.

Depois, a requisição vai para uma instância EC2, que verifica no RDS se o cliente já existe; se não existir, a EC2 faz o cadastro no banco.
