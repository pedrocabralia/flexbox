# Layout é a forma como os elementos estão distribuidos na tela 

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


     * Se eu quiser centralizar um elemento eu utilizo:

    ```css
           
              #normal{

                    margin: 0 auto;
                    width: 30px;
                }

    ```


  


   


