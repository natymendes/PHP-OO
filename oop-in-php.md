
```markdown
# OOP no PHP

O PHP oferece suporte completo à programação orientada a objetos, incluindo:
- **Construtores e Destrutores**: Métodos especiais usados na criação e destruição de objetos.
- **Modificadores de Acesso**: `public`, `private` e `protected`.
- **Namespace**: Organizam melhor o código.
- **Autoload**: Carrega automaticamente as classes.

```php
class Exemplo {
    public $nome;

    public function __construct($nome) {
        $this->nome = $nome;
    }

    public function saudacao() {
        return "Olá, " . $this->nome;
    }
}

$exemplo = new Exemplo("João");
echo $exemplo->saudacao();
