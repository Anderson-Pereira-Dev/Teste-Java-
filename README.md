# Teste-Java


### Questão 2

```
package br.com.teste.questao2
import java.util.Date;
import javax.persistence.Column;
import javax.persistence.Entity;
import javax.persistence.Id;
import javax.persistence.Table;

@Entity
@Table(name = "tb_veiculo")
public class Veiculo {
    @Id
    private String placa;

    @Column
    private String tipo;
   
    @Column
    private String cor;
    
    @Column
    private Date dataFabricacao;
}
```

### Questão 4

```
select * from alunos order by id

1	"Julia"	         81
2	"Carol"	         68
3	"Maria"	         99
4	"Andreia"	 78
5	"Jaqueline"	 63
6	"Marcela"	 88

```





### Questão 6 

```
public class Questao6 {

    public static void main(String[] args) {
        for(int numero = 1; numero <= 100; numero++) {
            if(numero % 3 == 0 && numero % 5 == 0) {
                System.out.println("FooBaa");
            } else if(numero % 3 == 0) {
                System.out.println("Foo");
            } else if(numero % 5 == 0) {
                System.out.println("Baa");
            } else {
                System.out.println(numero);
            }
        }
    }
}
```
