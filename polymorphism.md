
```markdown
# Polimorfismo

O polimorfismo permite que diferentes classes usem a mesma interface ou método de maneiras distintas.

```php
interface Animal {
    public function fazerSom();
}

class Cachorro implements Animal {
    public function fazerSom() {
        return "Latido";
    }
}

class Gato implements Animal {
    public function fazerSom() {
        return "Miado";
    }
}

function emitirSom(Animal $animal) {
    echo $animal->fazerSom();
}

emitirSom(new Cachorro());
emitirSom(new Gato());
