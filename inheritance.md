

```markdown
# Herança

A **herança** permite que uma classe herde as propriedades e métodos de outra classe.

```php
class Veiculo {
    public $marca;
    public $modelo;

    public function __construct($marca, $modelo) {
        $this->marca = $marca;
        $this->modelo = $modelo;
    }

    public function exibirDetalhes() {
        return "Marca: $this->marca, Modelo: $this->modelo";
    }
}

class Carro extends Veiculo {
    public $tipo;

    public function __construct($marca, $modelo, $tipo) {
        parent::__construct($marca, $modelo);
        $this->tipo = $tipo;
    }

    public function exibirDetalhes() {
        return parent::exibirDetalhes() . ", Tipo: $this->tipo";
    }
}

$meuCarro = new Carro("Toyota", "Corolla", "Sedan");
echo $meuCarro->exibirDetalhes();
