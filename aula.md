# Layout 
* é a forma como os elementos estão distribuidos na tela 

## Nomal Flow 

* São os elementos **block** e **inline**.
  
    ex: 
    ```html

           <p> Texto Block  <strong> inline</strong> </p>

            <p> texto block </p> 

    ```
     *colocar uma cor de fundo*   
    

* Dá para alterar o Css de Block para inline:
     
     ```css

       p{
             display: inline;
         }
   ```

## Table 

* É a forma de vizualização dos elementos em tabelas.  **tr** == linhas  e **td** == colunas.
    ex.: 
    ```html
        <table>
            <tr>
                <td>Nome:</td>
                <td>Pedro Vinicios</td>
            </tr>

            <tr>
                <td>idade:</td>
                <td>28</td>
            </tr>

        </table>

    ```


# Tabless

* A ideia aqui é não utilizar tabelas na organização dos elementos na tela.
    ex: 

    ```html
         <div id="esquerda">Esquerda</div>
         <div id="direita">Direita</div>
         <div id="normal">Normal</div>

     ```

     * No css:

         ```css
           
           #esquerda{

                float:left;
           }

           #direita{

                float: right;
            }

         ```


    * Se eu quiser que o próximo elemento se comporte normalmente eu coloco:

    ```css
           
            #normal{

                    clear: both;
                }

    ```


     * Centralizando um elemento:

    ```css
           
              #normal{

                    margin: 0 auto;
                    width: 30px;
                }

    ```


## FLEXBOX:

* É um forma de organizar os elementos na tela de forma mais dinâmica. Auxilinando na melhor,   **organização**, **alinhamento** e **distribuição** dos elementos.

 * ex no **HTML**:

 ```html
           
                    <div class="flexbox">
 
                        <div class="item">1</div>
                        <div class="item">2</div>
                        <div class="item">3</div>

                    </div>
```
* no **CSS**:

```css
           
                   .flexbox{
                                display: flex;
                                justify-content: space-around;
                            }
```

* Flex container é o elemento *pai* e os itens são os elementos filhos. 
* Outra terminologia utilizada é a de Nesting esse conceito quer dizer que um elemento vive dentro de outro.

* ex. no **HTML**:
```html
    <div class="container">
        <div class="item"></div>
        <div class="item"></div>
        <div class="item"></div>

    </div>
```
### Eixo (axis) principal e cruzado

* É A LINHA PELA QUAL IREMOS ALINHAR NOSSOS ÍTENS


![](img/mainAxis.png)[Referência](https://lucashenriquedeabreu.medium.com/flexbox-layout-a2ab0f0a2f86)

* Ex. no **HTML**:

```html

    <div class="container">
        <div class="item">A</div>
        <div class="item">B</div>
        <div class="item">C</div>

    </div>
```
no **CSS** alterando a posição em relação ao eixo principal:
```css
   .container{
    display: flex;
    justify-content: end;
}

```

* Podemos alterar a disposição dos itens para coluna, com isso alteramos também o eixo principal.

```css
    .container{
        display: flex;
        flex-direction: column;
        height: 500px;
        justify-content: end;

    }
```
### Flex sizing