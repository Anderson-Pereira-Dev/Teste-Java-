# Teste - Java - Radek 


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
SELECT * FROM FROM ALUNOS
ORDER BY ID

--RESULTADO DA CONSULTA:

1	"Julia"	         81
2	"Carol"	         68
3	"Maria"	         99
4	"Andreia"	 78
5	"Jaqueline"	 63
6	"Marcela"	 88

```

``` 
SELECT
CASE
WHEN VALOR < 70 THEN 'NULL' ELSE NOME END NOME,
CASE 
WHEN VALOR>=90 AND VALOR <=100 THEN 10
WHEN VALOR>=80 AND VALOR <=89 THEN 9
WHEN VALOR>=70 AND VALOR <=79 THEN 8
WHEN VALOR>=60 AND VALOR <=69 THEN 7
WHEN VALOR>=50 AND VALOR <=59 THEN 6
WHEN VALOR>=40 AND VALOR <=49 THEN 5
WHEN VALOR>=30 AND VALOR <=39 THEN 4
WHEN VALOR>=20 AND VALOR <=29 THEN 3
WHEN VALOR>=10 AND VALOR <=19 THEN 2
WHEN VALOR>=0 AND VALOR <=9 THEN 1 
END
AS NOTA,
VALOR
FROM ALUNOS
ORDER BY NOTA DESC, NOME DESC, VALOR


--RESULTADO DA CONSULTA :

"Maria" 	10	99
"Marcela"	9	88
"Julia"	        9	81
"Andreia"	8	78
"NULL"	        7	63
"NULL"	        7	68

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
