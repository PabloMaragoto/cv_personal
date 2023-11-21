# Muestra de código creado
## Repositorio Personal
[![Logotipo de github](img/github-mark.svg)](https://github.com/PabloMaragoto/conference-web)
## Lenguajes utilizados
- ### Java
    ```java
    import java.util.Scanner;

    public class creacionCuadrado{

	    static void cuadrado(int x, char y){
		    for(int j = 0; j < x ; j++){
			    if((j == 0) || (j == x-1)){
				    for(int k = 0; k< x; k++){
					    System.out.print(y+" ");
				    }
				    System.out.println();	
			    }else{
				    System.out.print(y + " ");
				    for(int l = 0; l < x -2; l++){
				    	System.out.print("  ");
				    }
				    System.out.print(y+" ");
				    System.out.println();
			    }
		    }
	    }
	    public static void main(String[] args){
		    Scanner sc = new Scanner(System.in);
		    int lado = sc.nextInt();
		    char material = sc.next().charAt(0);
		    cuadrado(lado, material);
		    sc.close();
	    }
    }
    ```
- ### HTML
    ```HTML
    <!DOCTYPE html>
    <html lang="en">
    <head>
        <meta charset="UTF-8">
        <meta http-equiv="X-UA-Compatible" content="IE=edge">
        <meta name="viewport" content="width=device-width, initial-scale=1.0">
        <link rel="shortcut icon" href="" type="image/x-icon">
        <link rel="shortcut icon" href="./img/favicon.ico" type="image/x-icon">
        <title>Order your burger</title>
    </head>
    <body>
        <header>
            <img src="./img/burger-svgrepo-com.svg" alt="Cute simply burger draw in cartoon style" width="200" height="150"/>
            <hr>
        </header>
        <main>
            <h1>Create a burger!</h1>
            <form action="burger.php" method="POST">
                <section>
                    <label for="protein">What type of protein would you like?</label>
                    <input type="text" name="protein" id="protein" value="nothing"/>
                    <hr>
                </section>
                <section>
                    <label for="patties">How many patties would you like?</label>
                    <input type="number" name="patties" id="patties" value="0" min="0" max="10">
                    <hr>
                </section>
                <section>
                    <label for="cooked">How do you want you patty cooked</label>
                    <p>Rare <input type="range" name="cooked" id="cooked" min="1" max="5" value="3"> Well-Cooked</p>
                    <hr>
                </section>
                <section>
                    What toppings would you like?
                    <br>
                    <label for="lettuce">Lettuce</label>
                    <input type="checkbox" name="lettuce" id="lettuce" value="lettuce">
                    <label for="tomato">Tomato</label>
                    <input type="checkbox" name="tomato" id="tomato" value="tomato">
                    <label for="onion">Onion</label>
                    <input type="checkbox" name="onion" id="onion" value="onion">
                    <hr>
                </section>
                <section>
                    Would you like to add cheese?
                    <br>
                    <label for="yes">Yes</label>
                    <input type="radio" name="cheese" id="yes" value="yes">
                    <label for="no">No</label>
                    <input type="radio" name="cheese" id="no" value="no">
                    <hr>
                </section>
                <section>
                    <label id="bun">What type of bun would you like?</label>
                    <select name="bun" id="bun">
                        <option value="sesamo">Sesame</option>
                        <option value="potato">Potato</option>
                        <option value="pretzel">Pretzel</option>
                    </select>
                    <hr>
                </section>
                <section>
                    <label id="sauce">What type of sauce would you like?</label>
                    <input type="text" list="listOfSauce" name="sauce" id="sauce" value="">
                    <datalist id="listOfSauce">
                        <option value="ketchup">Ketchup</option>
                        <option value="mayo">Mayo</option>
                        <option value="mostard">Mostard</option>
                        <option value="otherSauce">
                            <input type="text" name="otherSauce" id="otherSauce"/>
                        </option>
                        <option></option>
                    </datalist>
                    <hr>
                </section>
                <section>
                    <label id="addIngredient">Anything else you want to add?</label> <br>
                    <textarea id="addIngredient" name="addIngredient" cols="40" rows="4" value="nothing"></textarea>
                    <hr>
                </section>
                    <input type="submit" name="submit" id="submit">
                <section>  
                </section>
            </form>
        </main>
    </body>
    </html>
    ```

