# NetCatPy - Ferramenta de Rede em Python

**NetCatPy** é uma ferramenta desenvolvida em Python que simula o comportamento do NetCat, permitindo a transferência de dados, conexões a portas específicas e a criação de servidores ou clientes para comunicação em rede. Este projeto foi inspirado no livro *Black Hat Python* e busca ser uma alternativa simples para experimentos e aprendizado sobre redes.

---

## Recursos

- **Modo Cliente**: Conecte-se a servidores em portas específicas.
- **Modo Servidor**: Aguarde conexões de clientes e envie/receba mensagens.
- **Transferência de Arquivos**: Permite o envio e recebimento de arquivos entre hosts.
- **Flexível e Simples**: Fácil de usar e modificar para diferentes propósitos.

---

## Requisitos

- **Python 3.8 ou superior**
- Nenhuma biblioteca adicional é necessária.

---

## Instalação

1. Clone o repositório:
   ```bash
   git clone https://github.com/seu-usuario/NetCatPy.git
   ```

2. Navegue até o diretório do projeto:
   ```bash
   cd netcat
   ```

3. Execute o script principal:
   ```bash
   python netcat.py
   ```

---

## Uso

### Modo Cliente

Conecte-se a um servidor especificando o endereço IP e a porta:
```bash
python netcat.py -c -t <IP_SERVIDOR> -p <PORTA>
```
Exemplo:
```bash
python netcat.py -c -t 127.0.0.1 -p 8080
```

### Modo Servidor

Inicie o servidor em uma porta específica:
```bash
python netcat.py -s -p <PORTA>
```
Exemplo:
```bash
python netcat.py -s -p 8080
```

### Transferência de Arquivos

#### Envio de Arquivos
Cliente:
```bash
python netcat.py -c -t <IP_SERVIDOR> -p <PORTA> --send <CAMINHO_ARQUIVO>
```

#### Recebimento de Arquivos
Servidor:
```bash
python netcat.py -s -p <PORTA> --receive
```

---

## Opções Disponíveis

- `-c, --client`: Executa o NetCatPy no modo cliente.
- `-s, --server`: Executa o NetCatPy no modo servidor.
- `-t, --target`: Define o IP do servidor (modo cliente).
- `-p, --port`: Define a porta para conexão.
- `--send`: Envia um arquivo para o servidor.
- `--receive`: Recebe um arquivo no modo servidor.

---

## Contribuições

Contribuições são bem-vindas! Sinta-se à vontade para abrir issues ou enviar pull requests com melhorias e novas funcionalidades.

---

## Licença

Este projeto está licenciado sob a [Licença MIT](LICENSE).

---

## Contato

Se você tiver dúvidas ou sugestões, entre em contato:
- **Email**: seuemail@example.com
- **GitHub**: [seu-usuario](https://github.com/seu-usuario)

