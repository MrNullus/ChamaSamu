# ChamaSamu - Uma Biblioteca de Depuração PHP

A biblioteca **ChamaSamu** é uma ferramenta de depuração simples e útil para desenvolvedores PHP. Ela fornece métodos para exibir informações de depuração de maneira legível e organizada durante o desenvolvimento de aplicativos PHP. Essa biblioteca pode ser especialmente útil quando você precisa verificar o estado de variáveis, saídas de consultas SQL, conteúdo JSON ou XML, e muito mais, para entender melhor o comportamento de seu código.

## Recursos Principais

### Exibição de Saída de Depuração

- `debugPanel($data)`: Exibe uma janela flutuante contendo a saída de depuração formatada.
- `debug($data)`: Exibe a saída de depuração formatada em texto simples.
- `debugJSON($data)`: Exibe a saída de depuração formatada para JSON.
- `debugObject($object)`: Exibe a saída de depuração de um objeto em formato legível.
- `debugSQL($sql)`: Exibe a saída de depuração de uma consulta SQL.
- `debugMessage($message)`: Exibe a saída de depuração de mensagens personalizadas.
- `debugAssociativeArray($array)`: Exibe a saída de depuração de um array associativo com chave e valor.
- `debugBoolean($bool)`: Exibe a saída de depuração de uma variável booleana.
- `debugXML($data)`: Exibe a saída de depuração de uma variável em formato XML.
- `debugTable($data)`: Exibe a saída de depuração de uma variável em formato de tabela HTML.
- `debugList($data)`: Exibe a saída de depuração de uma variável em formato de lista HTML.

### Exibição de Dados de Requisição

- `session()`: Exibe a saída de depuração da sessão.
- `get()`: Exibe a saída de depuração do array GET.
- `post()`: Exibe a saída de depuração do array POST.

### Exibição de Código

- `code($code)`: Exibe a saída de depuração de código com formatação.

## Uso Básico

```php
use PunkSama\ChamaSamu\ChamaSamu;

// Exemplo de uso básico
$data = ['nome' => 'John', 'idade' => 30];
ChamaSamu::debug($data);

// Exemplo de exibição de saída de depuração JSON
$jsonData = '{"name": "John", "age": 30}';
ChamaSamu::debugJSON(json_decode($jsonData));

// Exemplo de exibição de saída de depuração de consulta SQL
$sql = 'SELECT * FROM users WHERE id = 1';
ChamaSamu::debugSQL($sql);
```

## Como Instalar

Você pode instalar a biblioteca **ChamaSamu** via Composer. Adicione o seguinte ao seu arquivo `composer.json`:

```json
{
    "require": {
        "punk-sama/chama-samu": "^1.0"
    }
}
```

Em seguida, execute `composer update` para instalar a biblioteca.

## Contribuições

Sinta-se à vontade para contribuir com melhorias, correções de bugs ou novos recursos para esta biblioteca. Você pode abrir problemas (issues) ou enviar pull requests no [repositório GitHub do ChamaSamu](https://github.com/punk-sama/ChamaSamu).

## Licença

A biblioteca **ChamaSamu** é distribuída sob a licença MIT. Consulte o arquivo `LICENSE` para obter detalhes.

---

Esperamos que a biblioteca **ChamaSamu** seja útil para você em seus projetos de desenvolvimento PHP. Se você tiver alguma dúvida, sugestão ou problema, não hesite em entrar em contato ou abrir uma issue no GitHub. Happy coding!
