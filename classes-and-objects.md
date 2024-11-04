# Classes e Objetos

Uma **classe** define a estrutura de um objeto. Um **objeto** é uma instância de uma classe.

```php
class Carro {
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

$meuCarro = new Carro("Toyota", "Corolla");
echo $meuCarro->exibirDetalhes();
