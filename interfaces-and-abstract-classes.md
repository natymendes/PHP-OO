
```markdown
# Interfaces e Classes Abstratas

- **Classes Abstratas**: Não podem ser instanciadas diretamente e podem conter métodos abstratos (sem implementação).
- **Interfaces**: Definem métodos que devem ser implementados por classes concretas.

```php
interface Transporte {
    public function mover();
}

class Carro implements Transporte {
    public function mover() {
        return "O carro está se movendo.";
    }
}
